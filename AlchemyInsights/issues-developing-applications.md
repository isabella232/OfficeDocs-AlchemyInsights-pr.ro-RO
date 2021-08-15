---
title: Probleme la dezvoltarea de aplicații
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013436"
---
# <a name="issues-developing-applications"></a>Probleme la dezvoltarea de aplicații

Pentru a depana cele mai obișnuite probleme atunci Azure Active Directory aplicații (AD), consultați următoarele articole:

- [Văd probleme la conectarea la aplicații utilizând doar browserul Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Nu știu cum să modific setările implicite pe durata de viață a tokenului pentru aplicația mea](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Sunt derutat despre modul în care funcționează consimțământul pentru aplicație](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Nu știu cum să acord permisiuni pentru aplicația mea](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Nu înțeleg diferența dintre permisiunile delegate și cele de aplicație](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Sfârșitul perioadei de asistență pentru Azure Active Directory de autentificare (ADAL) și Azure AD Graph API (AAD Graph)***

- Începând cu 30 iunie 2020, nu vom mai adăuga caracteristici noi la biblioteca de autentificare Azure Active Directory (ADAL) și Azure AD Graph API (AAD Graph). Vom continua să oferim asistență tehnică și actualizări de securitate, dar nu vom mai furniza actualizări de caracteristici.

- Începând cu 30 iunie 2022, vom înceta asistența pentru ADAL și AAD Graph, și nu vom mai furniza asistență tehnică sau actualizări de securitate. În urma acestei condiții, următoarele sunt implicațiile:

    - Aplicațiile care utilizează ADAL în versiunile de sistem de operare existente vor continua să funcționeze după această dată, dar nu vor primi asistență tehnică sau actualizări de securitate.

    - Este posibil ca aplicațiile care Graph AAD după această perioadă să nu mai primească răspunsuri de la punctele finale AAD Graph

**MigrareA ADAL**

Dacă utilizați aplicații Microsoft, vă recomandăm să actualizați la Biblioteca de autentificare Microsoft (MSAL), care are cele mai recente caracteristici și actualizări de securitate. Această recomandare este în contextul inițierii procesului de migrare a aplicațiilor sale la MSAL până la termenul limită de asistență. 

Migrarea de către Microsoft a aplicațiilor sale la MSAL asigură că aplicațiile beneficiază de securitatea permanentă și de îmbunătățirile în curs ale MSAL ale caracteristicilor.

1. [Citiți întrebările frecvente despre ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Aflați cum să efectuați migrarea aplicațiilor pe fiecare platformă](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Dacă aveți nevoie de ajutor pentru a înțelege care dintre aplicațiile dvs. utilizează ADAL, vă recomandăm să revizuiți codul sursă al tuturor aplicațiilor dvs. și, dacă este cazul, să contactați orice furnizori independenți de software (ISV) sau furnizori de aplicații. De asemenea, asistența Microsoft vă poate oferi o listă a tuturor aplicațiilor ADAL care nu provin de la Microsoft din entitatea găzduită.

**Migrarea AAD Graph**

Pentru aplicațiile care utilizează AAD Graph, urmați instrucțiunile noastre pentru a migra aplicațiile AAD Graph la Microsoft Graph:

1. [Lista noastră de verificarea migrării oferă un punct de pornire](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Portalul de înregistrare a aplicațiilor Azure afișează ce aplicații utilizează AAD Graph. Vă recomandăm să revizuiți codul sursă al tuturor aplicațiilor și, dacă este cazul, să contactați orice furnizor independent de software (ISV) sau furnizori de aplicații. Asistența Microsoft vă poate furniza, de asemenea, informații despre utilizarea Graph AAD în entitatea găzduită.







