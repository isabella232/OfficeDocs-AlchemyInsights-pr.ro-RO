---
title: Probleme la dezvoltarea de aplicații cu API-uri
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013472"
---
# <a name="issues-developing-applications-with-apis"></a>Probleme la dezvoltarea de aplicații cu API-uri

Pentru a începe să utilizați API Azure Active Directory Graph API, consultați Ghidul de pornire rapidă [Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) sau consultați documentația interactivă de referințe API Azure [AD Graph API.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Sfârșitul perioadei de asistență pentru Azure Active Directory de autentificare (ADAL) și Azure AD Graph API (AAD Graph)**

**Începând cu 30 iunie 2020,** nu vom mai adăuga caracteristici noi la aplicațiile ADAL și Azure AD Graph. Vom continua să oferim asistență tehnică și actualizări de securitate, dar nu vom mai furniza actualizări de caracteristici.

**Începând cu 30 iunie 2022,** vom încheia asistența pentru ADAL și Azure AD Graph și nu vom mai furniza asistență tehnică sau actualizări de securitate.

Aplicațiile care utilizează ADAL în versiunile de sistem de operare existente vor continua să funcționeze după această dată, dar nu vor primi asistență tehnică sau actualizări de securitate.

Este posibil ca aplicațiile care utilizează Azure AD Graph după această perioadă să nu mai primească răspunsuri de la centrul de administrare Azure AD Graph final.

**MigrareA ADAL**

Vă recomandăm să actualizați la [Biblioteca de autentificare Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), care are cele mai recente caracteristici și actualizări de securitate.

Dacă utilizați aplicații Microsoft, știți că Microsoft este în curs de migrare a aplicațiilor sale la MSAL până la termenul limită al perioadei de asistență, asigurându-se că vor beneficia de îmbunătățirile continue ale securității și caracteristicilor MSAL.

1. [Citiți întrebările frecvente despre ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Aflați cum să migrați aplicații pe fiecare platformă.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Dacă aveți nevoie de ajutor pentru a înțelege care dintre aplicațiile dvs. utilizează ADAL, vă recomandăm să revizuiți codul sursă al tuturor aplicațiilor dvs. și, dacă este cazul, să contactați orice isvs sau furnizori de aplicații. De asemenea, asistența Microsoft vă poate oferi o listă a tuturor aplicațiilor ADAL care nu provin de la Microsoft din entitatea găzduită.

**Migrarea AAD Graph**

Pentru aplicațiile care utilizează Azure AD Graph, urmați instrucțiunile noastre pentru a migra aplicațiile de [tip Graph Azure AD](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)la Microsoft Graph .

1. [Lista noastră de verificarea migrării oferă un punct de pornire](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Portalul de înregistrare a aplicațiilor Azure afișează ce aplicații utilizează AAD Graph. Vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor dvs. și, dacă este cazul, să contactați orice furnizor de software independent sau furnizor de aplicații. Asistența Microsoft vă poate furniza, de asemenea, o listă cu toate utilizările AAD Graph în entitatea găzduită.
1. Pentru ca aplicația dvs. să acceseze date în Microsoft Graph, utilizatorul sau administratorul trebuie să-i acorde permisiunile corecte printr-un proces de consimțământ. Referința [de Graph Microsoft listează](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) permisiunile asociate cu fiecare set major de API-uri Microsoft Graph microsoft. De asemenea, oferă instrucțiuni despre cum să utilizați permisiunile.
