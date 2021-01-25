---
title: Probleme cu dezvoltarea aplicațiilor cu API-uri
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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975015"
---
# <a name="issues-developing-applications-with-apis"></a>Probleme cu dezvoltarea aplicațiilor cu API-uri

Pentru a începe să utilizați API-ul Azure Active Directory Graph, consultați [Ghidul de pornire rapidă AZURE AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) sau vizualizați [documentația de referințe interactive AZURE AD Graph API](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Sfârșitul asistenței pentru Azure Active Directory Authentication Library (monica) și Azure AD Graph API (AAD Graph)**

**Începând cu 30 iunie 2020**, nu vom mai adăuga caracteristici noi la Monica și Azure AD Graph. Vom continua să oferim asistență tehnică și actualizări de securitate, dar nu vom mai furniza actualizări de caracteristici.

**Începând cu 30 iunie, 2022**, vom încheia asistența pentru monica și Azure AD Graph și nu va mai oferi asistență tehnică sau actualizări de securitate.

Aplicațiile care utilizează monica pe versiunile de sistem de operare existente vor continua să funcționeze după această dată, dar nu vor primi nicio asistență tehnică sau actualizări de securitate.

Aplicațiile care utilizează Azure AD Graph după această dată nu mai pot primi răspunsuri de la punctul final Azure AD Graph.

**Migrarea monica**

Vă recomandăm să actualizați la [biblioteca de autentificare Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), care are cele mai recente caracteristici și actualizări de securitate.

Dacă utilizați aplicațiile Microsoft, știți că Microsoft se află în procesul de migrare a aplicațiilor sale la MSAL până la termenul limită de finalizare a asistenței, pentru a se asigura că va beneficia de securitatea în curs de desfășurare și de îmbunătățiri ale caracteristicii MSAL.

1. [Citiți întrebările frecvente](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)despre Monica.
1. [Aflați cum să migrați aplicațiile pe o bază per platformă](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Dacă aveți nevoie de ajutor pentru a înțelege ce aplicații utilizați Monica, vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor și, dacă este cazul, să contactați orice ISV sau furnizori de aplicații. Asistența Microsoft vă poate oferi, de asemenea, o listă cu toate aplicațiile non-Microsoft Monica din entitatea găzduită.

**Migrarea graficului AAD**

Pentru aplicațiile care utilizează Azure AD Graph, urmați ghidul nostru pentru a migra [aplicațiile AZURE AD Graph la Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Lista de verificare a migrării oferă un punct de pornire](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Portalul de înregistrare Azure App Arată ce aplicații utilizează Dan Graph. Vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor și, dacă este cazul, să contactați orice ISV sau furnizori de aplicații. Asistența Microsoft vă poate oferi, de asemenea, o listă cu utilizarea tuturor grafurilor în entitatea găzduită.
1. Pentru ca aplicația să acceseze date în Microsoft Graph, utilizatorul sau administratorul trebuie să îi acorde permisiunile corecte printr-un proces de consimțământ. [Referințele pentru permisiunile Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) listează permisiunile asociate cu fiecare set principal de API-uri Microsoft Graph. De asemenea, furnizează instrucțiuni despre cum se utilizează permisiunile.
