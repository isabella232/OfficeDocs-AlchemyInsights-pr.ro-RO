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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063642"
---
# <a name="issues-with-authentication-libraries"></a>Probleme cu bibliotecile de autentificare

1. [Bibliotecile de autentificare a platformelor Microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) listează bibliotecile client și middleware compatibile Microsoft.
2. Biblioteca de autentificare Microsoft (MSAL) acceptă mai multe [fluxuri de autentificare](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) pentru utilizare în scenarii de aplicație diferite.
3. Pentru a autentifica și a achiziționa jetoane, inițializați o nouă aplicație publică sau confidențială pentru clientul dumneavoastră în cod. Puteți seta mai multe opțiuni de configurare atunci când inițializați aplicația client în biblioteca de autentificare Microsoft (MSAL). Pentru a afla mai multe, consultați [opțiunile de configurare a aplicațiilor](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Sfârșitul asistenței pentru Azure Active Directory Authentication Library (monica) și Azure AD Graph API (AAD Graph)**

**Începând cu 30 iunie 2020**, nu vom mai adăuga caracteristici noi la Monica și Azure AD Graph. Vom continua să oferim asistență tehnică și actualizări de securitate, dar nu vom mai furniza actualizări de caracteristici.

**Începând cu 30 iunie, 2022**, vom încheia asistența pentru monica și Azure AD Graph și nu va mai oferi asistență tehnică sau actualizări de securitate.

Aplicațiile care utilizează monica pe versiunile de sistem de operare existente vor continua să funcționeze după această dată, dar nu vor *primi nicio asistență tehnică sau actualizări de securitate*.

Aplicațiile care utilizează Azure AD Graph după această dată nu mai pot primi răspunsuri de la punctul final Azure AD Graph.

**Migrarea monica**

Vă recomandăm să actualizați la [Biblioteca de autentificare Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), care are cele mai recente caracteristici și actualizări de securitate.

Dacă utilizați aplicațiile Microsoft, știți că Microsoft se află în procesul de migrare a aplicațiilor sale la MSAL până la termenul limită de finalizare a asistenței, asigurându-vă că acestea vor beneficia de securitatea în curs de desfășurare și de îmbunătățiri ale caracteristicii MSAL.

Pentru mai multe informații, consultați:

1. [Citiți întrebările frecvente despre ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Aflați cum să efectuați migrarea aplicațiilor pe fiecare platformă](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Dacă aveți nevoie de ajutor pentru a înțelege ce aplicații utilizați Monica, vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor și, dacă este cazul, să contactați orice ISV sau furnizori de aplicații. De asemenea, asistența Microsoft vă poate oferi o listă a tuturor aplicațiilor ADAL care nu provin de la Microsoft din entitatea găzduită.

**Migrarea AAD Graph**

Pentru aplicațiile care utilizează Azure AD Graph, urmați ghidul nostru pentru a [migra aplicațiile AZURE AD Graph la Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Lista de verificare a migrării oferă un punct de pornire.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Portalul de înregistrare a aplicațiilor Azure afișează ce aplicații utilizează AAD Graph. Vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor dvs. și, dacă este cazul, să contactați orice furnizor de software independent sau furnizor de aplicații. Asistența Microsoft vă poate oferi, de asemenea, o listă cu utilizarea tuturor grafurilor în entitatea găzduită.
3. Pentru ca aplicația să acceseze date în Microsoft Graph, utilizatorul sau administratorul trebuie să îi acorde permisiunile corecte printr-un proces de consimțământ. [Referințele pentru permisiunile Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) listează permisiunile asociate cu fiecare set principal de API-uri Microsoft Graph. De asemenea, furnizează instrucțiuni despre cum se utilizează permisiunile.
