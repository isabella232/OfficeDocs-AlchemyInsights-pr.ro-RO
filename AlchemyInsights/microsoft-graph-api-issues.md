---
title: Probleme legate Graph API Microsoft
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975905"
---
# <a name="microsoft-graph-api-issues"></a>Probleme legate Graph API Microsoft

Acest subiect se poate aplica și dezvoltatorilor care utilizează în continuare Azure AD Graph API. Cu toate acestea, **se recomandă** ferm să utilizați Microsoft Graph pentru toate scenariile dvs. de gestionare a directorului, identității și accesului.

**Probleme de autentificare sau de autorizare**

- Dacă aplicația  dvs. nu poate obține simboluri pentru a apela Microsoft Graph, alegeți Problemă cu obținerea unui simbol de acces **(autentificare)** categoria Microsoft Graph pentru a obține ajutor și asistență mai specifice în acest subiect.
- Dacă aplicația dvs. primește **401 sau 403** erori **de** autorizare atunci când apelați Microsoft Graph, alegeți categoria Microsoft Graph API Obținere acces refuzat, pentru a obține ajutor și asistență mai specifice cu privire la acest subiect.

**Vreau să utilizez Microsoft Graph, dar nu sunt sigur de unde să încep**

- [Prezentare generală Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Prezentare generală a identității și a gestionării accesului în Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Noțiuni de bază despre construirea Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - testarea API-Graph Microsoft în entitatea găzduită sau într-o entitate găzduită de demonstrație

**Vreau să utilizez Microsoft Graph, dar acceptă API-urile director v1.0 de care am nevoie?**

Microsoft Graph API recomandat pentru gestionarea directoarelor, a identității și a accesului. Cu toate acestea, există încă câteva goluri între ceea ce este posibil în Azure AD Graph și Microsoft Graph. Examinați articolele următoare, care evidențiază cele mai recente diferențe care vă pot ajuta în alegerea dvs.:

- [Diferențele dintre tipurile de resurse, Graph Azure AD și Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Diferențe de proprietate între Azure AD Graph Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Diferențele de metodă dintre Azure AD și Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Api-ul pe care îl apelez nu funcționează - unde pot să testez mai mult?**

**Microsoft Graph Explorer** - testați API-urile Microsoft Graph din entitatea găzduită sau  dintr-o entitate găzduită de demonstrație și consultați interogările eșantion din Microsoft Graph Explorer.

**Aplicația mea este prea lentă și se amână. Ce îmbunătățiri pot face?**

În funcție de scenariu, există o varietate de opțiuni la dispoziția dvs. pentru a face aplicația mai performantă și, în unele cazuri, mai puțin predispusă la reglajul serviciului (atunci când efectuați prea multe apeluri).

- [Cele Graph bune practici Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Solicitări de procesare pe loturi](https://docs.microsoft.com/graph/json-batching)
- [Urmărirea modificărilor prin interogare delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Cum să fiți notificat cu privire la modificările aduse webhooks](https://docs.microsoft.com/graph/webhooks)
- [Instrucțiuni de throtare](https://docs.microsoft.com/graph/throttling)

**Unde pot găsi mai multe informații despre erori și probleme cunoscute?**

- [Microsoft Graph de răspuns la eroare](https://docs.microsoft.com/graph/errors)
- [Probleme cunoscute cu Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Unde pot verifica starea disponibilității și conectivității serviciului?**

Disponibilitatea serviciului și conectivitatea serviciilor subiacente care pot fi accesate prin intermediul Microsoft Graph pot afecta disponibilitatea generală și performanța Microsoft Graph.

- Pentru Azure Active Directory serviciilor, verificați starea serviciilor **de securitate + identitate** listate în pagina de stare [Azure.](https://azure.microsoft.com/status/)
- Pentru Office servicii care contribuie la Microsoft Graph, verificați starea serviciilor listate în tabloul de bord [cu starea serviciilor Office .](https://portal.office.com/adminportal/home#/servicehealth)

Erorile Graph autorizarea Microsoft pot fi generate de mai multe probleme diferite, cele mai multe generând o eroare 401 sau 403. De exemplu, următoarele pot duce la erori de autorizare:

- [Fluxuri de acces](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios) incorecte
- [Domenii de permisiune](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) incorect configurate
- Lipsa [consimțământului](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Sfârșitul perioadei de asistență pentru Azure Active Directory de autentificare (ADAL) și Azure AD Graph API (AAD Graph)***

**Începând cu 30 iunie 2020,** nu vom mai adăuga caracteristici noi la aplicațiile ADAL și Azure AD Graph. Vom continua să oferim asistență tehnică și actualizări de securitate, dar nu vom mai furniza actualizări de caracteristici.

**Începând cu 30 iunie 2022,** vom încheia asistența pentru ADAL și Azure AD Graph și nu vom mai furniza asistență tehnică sau actualizări de securitate.

Aplicațiile care utilizează ADAL pe versiunile de sistem de operare existente vor continua să funcționați după această perioadă, dar nu vor primi asistență *tehnică sau actualizări de securitate.*

Este posibil ca aplicațiile care utilizează Azure AD Graph după această perioadă să nu mai primească răspunsuri de la centrul de administrare Azure AD Graph final.

**MigrareA ADAL**

Vă recomandăm să actualizați la [Biblioteca de autentificare Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), care are cele mai recente caracteristici și actualizări de securitate.

Dacă utilizați aplicații Microsoft, știți că Microsoft este în curs de migrare a aplicațiilor sale la MSAL până la termenul limită de asistență, asigurându-se că va beneficia de îmbunătățirile continue ale securității și caracteristicilor MSAL.

1. [Citiți întrebările frecvente despre ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Aflați cum să efectuați migrarea aplicațiilor pe fiecare platformă](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Dacă aveți nevoie de ajutor pentru a înțelege care dintre aplicațiile dvs. utilizează ADAL, vă recomandăm să revizuiți codul sursă al tuturor aplicațiilor dvs. și, dacă este cazul, să contactați orice isvs sau furnizori de aplicații. De asemenea, asistența Microsoft vă poate oferi o listă a tuturor aplicațiilor ADAL care nu provin de la Microsoft din entitatea găzduită.

**Migrarea AAD Graph**

Pentru aplicațiile care utilizează Azure AD Graph, urmați instrucțiunile noastre pentru a migra [aplicațiile de E-mail Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)la Microsoft Graph .

1. [Lista noastră de verificarea migrării oferă un punct de pornire](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Portalul de înregistrare a aplicațiilor Azure afișează ce aplicații utilizează AAD Graph. Vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor dvs. și, dacă este cazul, să contactați orice furnizor de software independent sau furnizor de aplicații. Asistența Microsoft vă poate furniza, de asemenea, o listă cu toate utilizările AAD Graph în entitatea găzduită.
3. Pentru ca aplicația dvs. să acceseze date în Microsoft Graph, utilizatorul sau administratorul trebuie să-i acorde permisiunile corecte printr-un proces de consimțământ. Referința [de Graph Microsoft listează](https://docs.microsoft.com/graph/permissions-reference) permisiunile asociate cu fiecare set major de API-uri Microsoft Graph microsoft. De asemenea, oferă instrucțiuni despre cum să utilizați permisiunile.
