---
title: Problemă la resetarea parolei
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
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039978"
---
# <a name="problems-resetting-password"></a>Probleme cu resetarea parolei

Mai jos aveți câteva dintre problemele cu care vă puteți confrunta atunci când resetați parola și soluțiile posibile:

**Am o problemă cu resetarea parolei care nu este acoperită de celelalte categorii**

- Asigurați-vă că sunteți autorizat să resetați parolele. Numai administratorii globali, parolei și utilizatorii pot reseta parolele de utilizator. Administratorii globali pot reseta și parolele altor administratori privilegiați.
- Asigurați-vă că înțelegeți cerințele de licențiere:
    - Trebuie să aveți cel puțin o licență atribuită în organizația dvs.
        - Doar utilizatorii din cloud - Office 365 SKU cu plată O365 sau Azure AD Basic
        - Utilizatori în cloud și/sau locali - Azure AD Premium P1 sau P2, Enterprise Mobility + Security (EMS) sau Secure Productive Enterprise SPE)
        - Pentru a citi mai multe despre cerințele de licențiere, consultați articolul Cerințe de licențiere pentru resetarea parolei cu [autoservire Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Am probleme cu testarea politicii de resetare a parolei pe care am setat-o**

- Politicile aplicate recent pot dura câteva minute pentru a fi reproduse în toate centrele de date și punctele de final. Distanța fizică de la centrul de date va afecta și modul în care se aplică modificările rapid.
- Testați cu un utilizator final, nu cu un administrator și testați cu un set mic de utilizatori. Politicile configurate în portalul Azure se aplică DOAR pentru utilizatorii finali, nu pentru administratori. Microsoft impune o politică puternică de resetare a parolei cu două porți pentru orice rol de administrator Azure (de exemplu: Administrator global, Administrator de asistență, Administrator parole etc.)
    - Aflați mai [multe despre politicile pentru administratori.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Doresc să implementez resetarea parolei, dar nu doresc să le spun utilizatorilor să înregistreze informații de securitate suplimentare**

Prepopulați datele pentru utilizatorii dvs., astfel încât aceștia să nu fie trebuie să facă acest lucru! - Ca administrator, puteți seta proprietățile telefonului și ale e-mailului pentru utilizatori înainte de a începe resetarea parolei pentru organizația dvs. Puteți face acest lucru utilizând un api, PowerShell sau azure AD Conectare. Mai multe informații aici:
- [Implementarea resetării parolei fără a fi necesar ca utilizatorii să se înregistreze](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Ce date sunt utilizate pentru resetarea parolei](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Butonul de resetare a parolei este de culoare gri**

Nu sunteți autorizat să resetați parolele acestui utilizator. Numai administratorii globali, parolei și utilizatorii pot reseta parolele de utilizator. Administratorii globali pot reseta și parolele altor administratori privilegiați.

**Nu văd sistemul blade de resetare a parolei**

Nu sunteți autorizat să resetați parolele. Numai administratorii globali, parolei și utilizatorii pot reseta parolele de utilizator. Administratorii globali pot reseta și parolele altor administratori privilegiați.

**Nu văd integrarea blade la setările regionale pentru resetarea parolei**

- Integrarea blade regională se afișează numai în medii hibride, ceea ce înseamnă că utilizați writeback pentru parole pentru a manipula parolele utilizatorilor locali.
- Nu vedeți acest blade dacă:
    - Nu utilizați writebackul parolelor
    - Există o problemă cu instalarea/conectivitatea writebackului de parole
    - Există o problemă cu instalarea/conectivitatea Azure AD Conectare
    - Pentru mai mulți pași de depanare pentru problemele cu scrierea parolelor, consultați secțiunea [Depanarea writeback al parolelor](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nu știu cum să resetez parola unui utilizator**

1. Conectați-vă la portalul Azure ca administrator corespunzător.
1. Accesați blade Utilizatori și grupuri, selectați **Toți utilizatorii**.
1. Selectați un utilizator din listă.
1. Pentru utilizatorul selectat, selectați Prezentare **generală**, apoi, în bara de comenzi, faceți clic pe **Reinițializare parolă**.
1. Urmați instrucțiunile de pe ecran.
    - Resetări efectuate doar prin portalul Azure acceptă scrierea parolei.

**Resetez parola unui utilizator local din portalul Office 365 Admin sau din Office 365 mobilă, dar utilizatorul tot nu se poate conecta**

WriteBack de parole nu este acceptat în acest portal. Resetarea parolei de utilizator din nou în portalul Azure - portal.azure.com

