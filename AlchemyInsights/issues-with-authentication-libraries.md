---
title: Probleme cu bibliotecile de autentificare
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028016"
---
# <a name="issues-with-authentication-libraries"></a>Probleme cu bibliotecile de autentificare

1. [Serviciu de identitate Microsoft de autentificare listează](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) bibliotecile de client și de mijloc compatibile cu Microsoft.
2. Biblioteca de autentificare Microsoft (MSAL) acceptă mai multe fluxuri [de autentificare](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) pentru utilizare în scenarii de aplicație diferite.
3. Pentru a autentifica și a obține simboluri, inițializați o nouă aplicație client publică sau confidențială în cod. Puteți seta mai multe opțiuni de configurare atunci când inițializați aplicația client în Biblioteca de autentificare Microsoft (MSAL). Pentru a afla mai multe, consultați [Opțiuni de configurare a aplicației.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Sfârșitul perioadei de asistență pentru Azure Active Directory de autentificare (ADAL) și Azure AD Graph API (AAD Graph)**

**Începând cu 30 iunie 2020,** nu vom mai adăuga caracteristici noi la aplicațiile ADAL și Azure AD Graph. Vom continua să oferim asistență tehnică și actualizări de securitate, dar nu vom mai furniza actualizări de caracteristici.

**Începând cu 30 iunie 2022,** vom încheia asistența pentru ADAL și Azure AD Graph și nu vom mai furniza asistență tehnică sau actualizări de securitate.

Aplicațiile care utilizează ADAL pe versiunile de sistem de operare existente vor continua să funcționați după această perioadă, dar nu vor primi asistență *tehnică sau actualizări de securitate.*

Este posibil ca aplicațiile care utilizează Azure AD Graph după această perioadă să nu mai primească răspunsuri de la centrul de administrare Azure AD Graph final.

**MigrareA ADAL**

Vă recomandăm să actualizați la [Biblioteca de autentificare Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), care are cele mai recente caracteristici și actualizări de securitate.

Dacă utilizați aplicații Microsoft, știți că Microsoft este în curs de migrare a aplicațiilor sale la MSAL până la termenul limită de asistență, asigurându-se că va beneficia de îmbunătățirile continue ale securității și caracteristicilor MSAL.

Pentru mai multe informații, consultați:

1. [Citiți întrebările frecvente despre ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Aflați cum să efectuați migrarea aplicațiilor pe fiecare platformă](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Dacă aveți nevoie de ajutor pentru a înțelege care dintre aplicațiile dvs. utilizează ADAL, vă recomandăm să revizuiți codul sursă al tuturor aplicațiilor dvs. și, dacă este cazul, să contactați orice isvs sau furnizori de aplicații. De asemenea, asistența Microsoft vă poate oferi o listă a tuturor aplicațiilor ADAL care nu provin de la Microsoft din entitatea găzduită.

**Migrarea AAD Graph**

Pentru aplicațiile care utilizează Azure AD Graph, urmați instrucțiunile noastre pentru a migra [aplicațiile de E-mail Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)la Microsoft Graph .

1. [Lista noastră de verificare pentru migrare oferă un punct de plecare.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Portalul de înregistrare a aplicațiilor Azure afișează ce aplicații utilizează AAD Graph. Vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor dvs. și, dacă este cazul, să contactați orice furnizor de software independent sau furnizor de aplicații. Asistența Microsoft vă poate furniza, de asemenea, o listă cu toate utilizările AAD Graph în entitatea găzduită.
3. Pentru ca aplicația dvs. să acceseze date în Microsoft Graph, utilizatorul sau administratorul trebuie să-i acorde permisiunile corecte printr-un proces de consimțământ. Referința [de Graph Microsoft listează](https://docs.microsoft.com/graph/permissions-reference) permisiunile asociate cu fiecare set major de API-uri Microsoft Graph microsoft. De asemenea, oferă instrucțiuni despre cum să utilizați permisiunile.
