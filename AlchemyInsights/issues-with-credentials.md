---
title: Probleme cu acreditările
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986831"
---
# <a name="issues-with-credentials"></a>Probleme cu acreditările

Serviciu de identitate Microsoft și fluxul de acreditări de [client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) descrie cum se programează direct în raport cu acreditările de client OAuth 2.0.

**Cum gestionez parola sau acreditările unui certificat de aplicație?**

În Azure CLI, puteți utiliza acreditările aplicației [Az Ad](https://docs.microsoft.com/cli/azure/ad/app/credential) pentru a șterge, a lista sau a reseta parola sau acreditările unui certificat de aplicație.

**Cum își resetează utilizatorii parolele?**

Utilizatorii trebuie să [se înregistreze pentru resetarea cu autoservizare](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) a parolelor înainte de a-și putea reseta parolele. După ce un utilizator s-a înregistrat, poate urma instrucțiunile din acest articol pentru a-și reseta parola: [Resetarea parolei de la locul de muncă sau de la școală.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Cum își modifică utilizatorii parolele?**

Utilizatorii pot urma pașii din acest articol pentru a-și modifica [parolele: Cum să vă modificați parola.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
De asemenea, [aceștia pot gestiona parolele de aplicații pentru verificarea în doi pași.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Utilizatorul meu primi o eroare atunci când modifică sau reinițialează parola sa**

Acest link va furniza informații despre problemele uzuale care pot apărea atunci când un utilizator încearcă să își reseteze parola: [Probleme comune și soluțiile la acesta](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Am o problemă la resetarea parolei unui utilizator**

- Asigurați-vă că sunteți autorizat să resetați parolele. *Numai administratorii globali, parolei și utilizatorii pot reseta parolele de utilizator.* Administratorii globali pot reseta și parolele altor administratori privilegiați.

- Asigurați-vă că înțelegeți cerințele de licențiere:

  - Trebuie să aveți cel puțin o licență atribuită în organizația dvs.:
    - **Doar utilizatorii din** cloud - orice SKU cu plată Office 365 (O365) sau Azure AD Basic
    - **Utilizatori în cloud și/sau** locali - Azure AD Premium P1 sau P2, Enterprise Mobility + Security (EMS) sau Secure Productive Enterprise (SPE)
    - Pentru a afla mai multe despre cerințele de licențiere, consultați [Cerințe de licențiere pentru resetarea parolei cu autoservire Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Pentru a reseta parola unui utilizator, găsiți utilizatorul în Azure AD. Apoi, pe blade de prezentare generală pentru acel utilizator, faceți clic pe butonul "resetați parola".

**Butonul de resetare a parolei este de culoare gri**

Nu sunteți autorizat să **resetați** parolele acestui utilizator. *Numai administratorii globali, parolei și utilizatorii pot reseta parolele de utilizator.* Administratorii globali pot reseta și parolele altor administratori privilegiați.

**Nu văd sistemul blade de resetare a parolei**

Nu sunteți autorizat să resetați parolele. *Numai administratorii globali, parolei și utilizatorii pot reseta parolele de utilizator.* Administratorii globali pot reseta și parolele altor administratori privilegiați.

**Nu văd integrarea blade la setările regionale pentru resetarea parolei**

- Integrarea blade regională se afișează numai în medii hibride, ceea ce înseamnă că utilizați writeback pentru parole pentru a manipula parolele utilizatorilor locali.

- Nu vedeți acest blade dacă:

  - Nu utilizați writebackul parolelor
  - Există o problemă cu instalarea/conectivitatea writebackului de parole
  - Există o problemă cu instalarea/conectivitatea Azure AD Conectare
  - Pentru mai mulți pași de depanare pentru problemele cu scrierea parolelor, consultați [Depanarea writeback a parolelor](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Nu știu cum să resetez parola unui utilizator**

1. Conectați-vă la portalul Azure ca administrator corespunzător.
2. Accesați blade Utilizatori **și grupuri,** selectați **Toți utilizatorii**.
3. Selectați un utilizator din listă.
4. Pentru utilizatorul selectat, selectați Prezentare **generală**, apoi, în bara de comenzi, selectați **Reinițializare parolă**.
5. Selectați **butonul Resetați** parola și urmați instrucțiunile de pe ecran.
    - Resetări efectuate doar prin portalul **Azure acceptă** scrierea parolei.

**Resetez parola unui utilizator local din portalul Office 365 Admin sau din Office 365 mobilă, dar utilizatorul tot nu se poate conecta**

WriteBack de parole nu este acceptat în acest portal. Reinițializați parola utilizatorului din nou în portalul Azure.
