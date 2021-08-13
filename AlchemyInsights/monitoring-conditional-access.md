---
title: Monitorizarea accesului condiționat
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975113"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorizarea accesului condiționat pentru Exchange

Utilizatorii țintiți cu acces condiționat vor primi un e-mail de notificare dacă nu îndeplinesc cerințele de acces ale organizației dvs. Pentru a rezolva problema, vă recomandăm una sau mai multe dintre următoarele soluții:

- Dacă dispozitivul trebuie să fie înregistrat, sfătuiți utilizatorul să meargă la aplicația Portal firmă și să verifice dacă apare în Portal firmă. Dacă nu, utilizatorul trebuie să înscrie dispozitivul.
- În portalul Azure, accesați Intune > Conformitate dispozitiv. Sub Monitor, faceți clic pe Conformitate dispozitiv. Vizualizați raportul de conformitate al dispozitivului pentru a verifica dacă dispozitivul utilizatorului este marcat drept compatibil.
- În portalul Azure, accesați Intune > Conformitate dispozitiv. Sub Gestionare, faceți clic pe Politici. În lista cu politicile de conformitate, verificați dacă s-a atribuit un profil pentru dispozitivul utilizatorului. Dacă nu i s-a atribuit niciun profil, Intune nu va putea să confirme starea de conformitate a dispozitivului.
- Editați atribuirea de acces condiționat a utilizatorului.

1. În portalul Azure, accesați Politici **de acces condiționat Intune.**  >    >  
2. Selectați o politică din listă.
3. Faceți clic pe Utilizatori și grupuri.
4. Pentru a direcționa o politică anume către o persoană, adăugați persoana în lista Includere. Pentru a asigura că o persoană este omisă de la o politică, adăugați persoana în lista Excludere.

Linkuri utile:

[Prezentarea generală a conformității dispozitivului](https://docs.microsoft.com/intune/device-compliance-get-started)

[Depanarea CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Politică de depanare](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Monitorizarea conformității dispozitivului Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Notă: acești pași sunt utili doar pentru depanarea accesului Azure Active Directory caracteristică condiționată. De asemenea, este posibil să puneți în carantină un dispozitiv care blochează accesul la e-mail Exchange dvs. Mai multe informații despre Exchange de management al dispozitivelor pot fi găsite [aici]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
