---
title: Monitorizarea accesului condiționat Intune
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
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327569"
---
# <a name="monitor-intune-conditional-access"></a>Monitorizarea accesului condiționat Intune

Utilizatorii țintiți cu acces condiționat vor primi un e-mail de notificare dacă nu îndeplinesc cerințele de acces ale organizației dvs. Pentru a rezolva problema, vă recomandăm una sau mai multe dintre următoarele soluții:

1. Dacă dispozitivul trebuie să fie înregistrat, sfătuiți utilizatorul să meargă la aplicația Portal firmă și să verifice dacă apare în Portal firmă. Dacă nu, utilizatorul trebuie să înscrie dispozitivul.
1. În portalul Azure, accesați **Conformitatea dispozitivului Intune.**  >   
1. Pentru a vedea raportul de conformitate al dispozitivului pentru a verifica dacă dispozitivul utilizatorului este marcat drept compatibil, sub **Monitor,** faceți clic **pe Conformitate dispozitiv.**
1. În portalul Azure, accesați **Conformitatea dispozitivului Intune.**  >   Sub **Gestionare, faceți** **clic pe Politici.** În lista cu politicile de conformitate, verificați dacă s-a atribuit un profil pentru dispozitivul utilizatorului. Dacă nu i s-a atribuit niciun profil, Intune nu va putea să confirme starea de conformitate a dispozitivului.
1. Editați atribuirea de acces condiționat a utilizatorului.
1. În portalul Azure, navigați la Politici de acces condiționat **Intune,** selectați o politică din listă  >    >  și faceți clic **pe Utilizatori și grupuri.**
1. Pentru a direcționa o politică anume către o persoană, adăugați persoana în **lista Includere.** Pentru a asigura că o persoană este omisă de la o politică, adăugați persoana în **lista Excludere.**

**Linkuri utile:**

- [Prezentarea generală a conformității dispozitivului](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Depanarea CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Politică de depanare](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Monitorizarea conformității dispozitivului Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Notă:** Acești pași sunt utili doar pentru depanarea accesului condiționat Azure Active Directory caracteristică condiționată. De asemenea, este posibil să puneți în carantină un dispozitiv care blochează accesul la e-mail Exchange dvs. Mai multe informații despre managementul Exchange dispozitive pot fi găsite [**aici.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
