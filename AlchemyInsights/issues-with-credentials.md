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
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063685"
---
# <a name="issues-with-credentials"></a>Probleme cu acreditările

[Platforma de identitate Microsoft și fluxul de acreditări client 2,0 OAuth](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) descrie cum să programați direct împotriva fluxului de acordare a acreditărilor client OAuth 2,0.

**Cum gestionez parola sau acreditările de certificat ale unei aplicații?**

În CLI-ul Azure, puteți să utilizați [acreditarea aplicației de publicitate AZ](https://docs.microsoft.com/cli/azure/ad/app/credential) pentru a șterge, a enumera sau a reinițializa acreditările de certificat sau parola unei aplicații.

**Cum își reinițializează utilizatorii parolele?**

Utilizatorii trebuie să se [înregistreze pentru resetarea parolei cu autoservire](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) înainte să își poată reseta parolele. După ce un utilizator s-a înregistrat, aceștia pot urmări instrucțiunile din acest articol pentru a-și reseta parola: [resetarea parolei de la locul de muncă sau de la școală](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Cum își modifică utilizatorii parolele?**

Utilizatorii pot urma pașii din acest articol pentru a-și schimba parolele: [cum să vă modificați parola](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
De asemenea, pot [gestiona parole de aplicație pentru verificarea în doi pași](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Utilizatorul meu primește o eroare la modificarea sau resetarea parolei**

Acest link va furniza informații despre problemele comune care pot apărea atunci când un utilizator încearcă să își reseteze parola: [probleme comune și soluțiile lor](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Am o problemă la reinițializarea parolei unui utilizator**

- Asigurați-vă că sunteți autorizat să resetați parole. *Doar administratorii globali, parole și utilizatori pot reseta parole de utilizator.* Administratorii globali pot reseta și alte parole ale administratorului privilegiat.

- Asigurați-vă că înțelegeți cerințele de licențiere:

  - Trebuie să aveți cel puțin o licență atribuită în organizația dvs.:
    - **Utilizatori Cloud Only** -orice Office 365 (O365) a plătit SKU sau Azure AD Basic
    - **Utilizatori cloud și/sau locali** -Azure AD Premium P1 sau P2, Enterprise Mobility + Security (EMS) sau Secure productive Enterprise (SPE)
    - Pentru a afla mai multe despre cerințele de licențiere, consultați [cerințe de licențiere pentru resetarea parolei AZURE AD self-service](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Pentru a reseta parola unui utilizator, găsiți utilizatorul în Azure AD. Apoi, pe lama generală pentru acel utilizator, faceți clic pe butonul "Reinițializare parolă".

**Butonul de resetare a parolei este estompat**

Nu sunteți autorizat să resetați parolele **acestui** utilizator. *Doar administratorii globali, parole și utilizatori pot reseta parole de utilizator.* Administratorii globali pot reseta și alte parole ale administratorului privilegiat.

**Nu văd lama de resetare a parolei**

Nu sunteți autorizat să resetați parole. *Doar administratorii globali, parole și utilizatori pot reseta parole de utilizator.* Administratorii globali pot reseta și alte parole ale administratorului privilegiat.

**Nu văd lama de integrare locală în resetarea parolei**

- Lama de integrare locală apare doar în medii hibride, ceea ce înseamnă că utilizați parole writeback pentru a manipula parolele utilizatorilor locali.

- Nu vedeți această lamă dacă:

  - Nu utilizați parola writeback
  - Există o problemă cu instalarea/conectivitatea parolei writeback
  - Există o problemă cu instalarea/conectivitatea Azure AD Connect
  - Pentru mai mulți pași de depanare pentru problemele cu parola writeback, consultați [Depanarea parolei writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Nu știu cum să resetez parola unui utilizator**

1. Conectați-vă la portalul Azure ca administrator corespunzător.
2. Accesați lama **utilizatori și grupuri** , selectați **toți utilizatorii**.
3. Selectați un utilizator din listă.
4. Pentru utilizatorul selectat, selectați **Prezentare generală**, apoi, în bara de comenzi, selectați **Reinițializare parolă**.
5. Selectați butonul **Reinițializare parolă** și urmați instrucțiunile de pe ecran.
    - Se resetează doar prin intermediul parolei de asistență writeback pentru **portalul Azure** .

**Am reinițializat o parolă de utilizator locală din portalul de administrare Office 365 sau din aplicația mobilă Office 365, dar utilizatorul încă nu se poate conecta**

Writeback parolelor nu este acceptată în acest portal. Reinițializați parola utilizatorului în portalul Azure.
