---
title: Problemă la reinițializarea parolei
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696275"
---
# <a name="problems-resetting-password"></a>Probleme la resetarea parolei

În continuare, există câteva dintre problemele cu care ați putea face față atunci când reinițializați parola și soluțiile posibile:

**Am o problemă cu resetarea parolei care nu este acoperită în celelalte categorii**

- Asigurați-vă că sunteți autorizat să resetați parole. Doar administratorii globali, parole și utilizatori pot reseta parole de utilizator. Administratorii globali pot reseta și alte parole ale administratorului privilegiat.
- Asigurați-vă că înțelegeți cerințele de licențiere:
    - Trebuie să aveți cel puțin o licență atribuită în organizația dvs.
        - Utilizatori Cloud Only-orice Office 365 (O365) a plătit SKU sau Azure AD Basic
        - Utilizatori cloud și/sau locali-Azure AD Premium P1 sau P2, Enterprise Mobility + Security (EMS) sau Secure productive Enterprise (SPE)
        - Pentru a citi mai multe despre cerințele de licențiere, consultați articolul [cerințele de licențiere pentru resetarea parolei AZURE AD self-service](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**Am probleme la testarea politicii de resetare a parolei setate**

- Politicile aplicate recent pot dura câteva minute pentru a se reproduce în toate centrele de date și punctele finale. Distanța fizică de la centrul de date va afecta, de asemenea, cât de repede se aplică modificările.
- Testați cu un utilizator final, nu cu un administrator și pilot cu un set mic de utilizatori. Politicile configurate în portalul Azure se aplică doar pentru utilizatorii finali, nu pentru administratori. Microsoft impune o politică de resetare a parolei cu două porți implicite pentru orice rol de administrator Azure (exemplu: administrator global, administrator Helpdesk, administrator de parole etc.)
    - Aflați mai multe despre [politicile pentru administratori](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Doresc să lansez resetarea parolei, dar nu doresc să fac ca utilizatorii mei să înregistreze informații suplimentare de securitate**

Pre-popula date pentru utilizatori, astfel încât aceștia să nu fie nevoiți! -În calitate de administrator, puteți seta proprietățile telefonului și e-mailului pentru utilizatori înainte de a reinițializa parola la organizația dvs. Puteți face acest lucru utilizând un API, PowerShell sau Azure AD Connect. Mai multe informații aici:
- [Implementarea resetării parolei fără a solicita utilizatorilor să se înregistreze](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Ce date se utilizează prin resetarea parolei](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Butonul de resetare a parolei este estompat**

Nu sunteți autorizat să resetați parolele acestui utilizator. Doar administratorii globali, parole și utilizatori pot reseta parole de utilizator. Administratorii globali pot reseta și alte parole ale administratorului privilegiat.

**Nu văd lama de resetare a parolei**

Nu sunteți autorizat să resetați parole. Doar administratorii globali, parole și utilizatori pot reseta parole de utilizator. Administratorii globali pot reseta și alte parole ale administratorului privilegiat.

**Nu văd lama de integrare locală în resetarea parolei**

- Lama de integrare locală apare doar în medii hibride, ceea ce înseamnă că utilizați parole writeback pentru a manipula parolele utilizatorilor locali.
- Nu vedeți această lamă dacă:
    - Nu utilizați parola writeback
    - Există o problemă cu instalarea/conectivitatea parolei writeback
    - Există o problemă cu instalarea/conectivitatea Azure AD Connect
    - Pentru mai mulți pași de depanare pentru problemele cu parola writeback, consultați secțiunea [Depanarea parolei writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nu știu cum să resetez parola unui utilizator**

1. Conectați-vă la portalul Azure ca administrator corespunzător.
1. Accesați lama utilizatori și grupuri, selectați **toți utilizatorii**.
1. Selectați un utilizator din listă.
1. Pentru utilizatorul selectat, selectați **Prezentare generală**, apoi, în bara de comenzi, faceți clic pe **Reinițializare parolă**.
1. Urmați instrucțiunile de pe ecran.
    - Se resetează doar prin intermediul parolei de asistență writeback pentru portalul Azure.

**Am reinițializat o parolă de utilizator locală din portalul de administrare Office 365 sau din aplicația mobilă Office 365, dar utilizatorul încă nu se poate conecta**

Writeback parolelor nu este acceptată în acest portal. Resetarea parolei utilizatorului din nou în portalul Azure-portal.azure.com

