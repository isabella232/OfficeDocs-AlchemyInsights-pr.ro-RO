---
title: Probleme cu dezvoltarea aplicațiilor
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
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974770"
---
# <a name="issues-developing-applications"></a>Probleme cu dezvoltarea aplicațiilor

Pentru a depana problemele cele mai comune atunci când construiți aplicații Azure Active Directory (AD), consultați următoarele articole:

- [Văd probleme la conectarea la aplicații folosind doar browserul Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Nu știu cum să modific valorile implicite pentru durata de viață a tokenului pentru aplicația mea](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Sunt confuz în legătură cu modul în care funcționează consimțământul aplicației](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Nu știu cum să acord permisiuni aplicației mele](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Nu înțeleg diferența dintre permisiunile delegate și aplicație](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Sfârșitul asistenței pentru Azure Active Directory Authentication Library (monica) și AZURE AD Graph API (AAD Graph)** _

- Începând cu 30 iunie, 2020, nu vom mai adăuga caracteristici noi la Azure Active Directory Authentication Library (monica) și Azure AD Graph API (AAD Graph). Vom continua să oferim asistență tehnică și actualizări de securitate, dar nu vom mai furniza actualizări de caracteristici.

- Începând cu 30 iunie, 2022, vom încheia suportul pentru monica și Dan grafic și nu va mai furniza asistență tehnică sau actualizări de securitate. Ca rezultat al acestei condiții, sunt implicați următoarele:

    - Aplicațiile care utilizează monica pe versiunile de sistem de operare existente vor continua să funcționeze după această dată, dar nu vor primi nicio asistență tehnică sau actualizări de securitate.

    - Este posibil ca aplicațiile care utilizează Dan Graph să nu mai primească răspunsuri de la punctul final din punct grafic

-*Migrarea* monica*

Dacă utilizați aplicațiile Microsoft, vă recomandăm să actualizați la biblioteca de autentificare Microsoft (MSAL), care are cele mai recente caracteristici și actualizări de securitate. Această recomandare este în contextul Microsoft inițiază procesul de migrare a aplicațiilor sale la MSAL până la termenul limită de finalizare a asistenței. 

Migrarea de la Microsoft a aplicațiilor sale către MSAL asigură faptul că aplicațiile beneficiază de îmbunătățiri de securitate și caracteristici ale MSAL.

1. [Citiți întrebări frecvente despre Monica](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Aflați cum să migrați aplicațiile pe o bază per platformă](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Dacă aveți nevoie de ajutor pentru a înțelege ce aplicații utilizați Monica, vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor și, dacă este cazul, să luați legătura cu orice vânzători de software independenți (ISV) sau furnizori de aplicații. Asistența Microsoft vă poate oferi, de asemenea, o listă cu toate aplicațiile non-Microsoft Monica din entitatea găzduită.

**Migrarea graficului AAD**

Pentru aplicațiile care utilizează Dan Graph, urmați ghidul nostru pentru a migra aplicațiile cu un grafic AAD la Microsoft Graph:

1. [Lista de verificare a migrării oferă un punct de pornire](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Portalul de înregistrare Azure App Arată ce aplicații utilizează Dan Graph. Vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor și, dacă este cazul, să contactați vânzătorii de software independenți (ISV) sau furnizorii de aplicații. Asistența Microsoft vă poate oferi, de asemenea, informații despre utilizarea în Graph a graficului în entitatea găzduită.







