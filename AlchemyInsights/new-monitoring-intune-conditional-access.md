---
title: Monitorizarea accesului condițional al Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427927"
---
# <a name="monitor-intune-conditional-access"></a>Monitorizarea accesului condițional al Intune

Utilizatorii vizați de Access condițional vor primi un e-mail de notificare dacă nu îndeplinesc cerințele de acces ale organizației dvs. Pentru a rezolva, vă recomandăm una sau mai multe dintre următoarele soluții:

1. Dacă se presupune că dispozitivul este înscris, consiliați utilizatorul să meargă la aplicația portal a firmei și să verifice dacă apare în portalul firmei. Dacă nu, utilizatorul trebuie să înscrie dispozitivul.
1. În portalul Azure, accesați   >  **conformitatea dispozitivelor** Intune. 
1. Pentru a vedea raportul de conformitate al dispozitivului pentru a verifica dacă dispozitivul utilizatorului este marcat ca fiind conform, sub **Monitor**, faceți clic pe **conformitate dispozitiv**.
1. În portalul Azure, accesați   >  **conformitatea dispozitivelor** Intune. Sub **gestionare,** faceți clic pe **politici**. În lista de politici de conformitate, Verificați dacă un profil este atribuit dispozitivului utilizatorului. Dacă nu este atribuit niciun profil, atunci Intune nu va putea confirma starea de conformitate a dispozitivului.
1. Editați atribuirea accesului condiționat al utilizatorului.
1. În portalul Azure, navigați la politicile de   >  **acces condiționale** Intune  >  , selectați o politică din listă și faceți clic pe **utilizatori și grupuri**.
1. Pentru a viza o anumită politică la o persoană, adăugați-o la **lista includere**. Pentru a vă asigura că o persoană este omisă din politică, adăugați-o la **lista de excluderi**.

**Linkuri utile:**

- [Prezentare generală a conformității dispozitivelor](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Depanarea CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Politica de depanare](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Monitorizarea conformității dispozitivelor Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Acești pași sunt utili doar pentru depanarea caracteristicii Azure Active Directory Access condiționale. De asemenea, este posibil să plasați în carantină un dispozitiv care blochează accesul la e-mail cu politica Exchange. Mai multe informații despre gestionarea dispozitivelor Exchange pot fi găsite [**aici**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
