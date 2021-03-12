---
title: Probleme cu API-ul Microsoft Graph
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
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714157"
---
# <a name="microsoft-graph-api-issues"></a>Probleme cu API-ul Microsoft Graph

Acest subiect se poate aplica și pentru dezvoltatori care utilizează încă Azure AD Graph API. Cu toate acestea, se recomandă **insistent** să utilizați Microsoft Graph pentru toate scenariile de gestionare a directorului, identității și Access.

**Probleme de autentificare sau de autorizare**

- Dacă aplicația **nu reușește să obțină tokenuri** pentru a apela Microsoft Graph, alegeți **problema cu obținerea unei categorii de simboluri Access (autentificare)** Microsoft Graph pentru a obține ajutor și asistență specifice pentru acest subiect.
- În cazul în care aplicația **primește erori de autorizare 401 sau 403** atunci când apelare Microsoft Graph, alegeți categoria **Obțineți o eroare Access Denied (autorizare)** Microsoft Graph API pentru a obține ajutor și asistență specifice în acest articol.

**Doresc să utilizez Microsoft Graph, dar nu sunt sigur de unde să încep**

- [Prezentare generală a Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Prezentare generală a identității și gestionării accesului în Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Introducere în construirea aplicațiilor Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** -testați API-uri Microsoft Graph în entitatea găzduită sau într-o entitate găzduită demo

**Doresc să utilizez Microsoft Graph, dar acceptă API-urile de directoare v 1.0 de care am nevoie?**

Microsoft Graph este API-ul recomandat pentru directorul, identitatea și gestionarea accesului. Cu toate acestea, există încă câteva lacune între ceea ce este posibil în Azure AD Graph și Microsoft Graph. Revizuiți următoarele articole, care evidențiază cele mai recente diferențe de asistență în alegerea dvs.:

- [Diferențele de tip de resursă între Azure AD Graph și Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Diferențe de proprietăți între Azure AD Graph și Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Diferențe de metodă între Azure AD și Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Interfața API pe care o apelez nu funcționează-unde pot face mai multe teste?**

**Microsoft Graph Explorer** -testați API-uri Microsoft Graph în entitatea găzduită sau într-o entitate găzduită demo și consultați și **interogările eșantion** din Microsoft Graph Explorer.

**Aplicația mea este prea lentă și, de asemenea, este accelerat. Ce îmbunătățiri pot să fac?**

În funcție de scenariul dvs., există o varietate de opțiuni la dispoziție pentru a face aplicația mai performantă și, în unele cazuri, mai puțin predispus la a fi accelerat de serviciu (atunci când efectuați prea multe apeluri).

- [Cele mai bune practici Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Solicitări de grupare](https://docs.microsoft.com/graph/json-batching)
- [Urmărirea modificărilor prin Delta Query](https://docs.microsoft.com/graph/delta-query-overview)
- [Fiți notificat de modificări prin intermediul cârligelor](https://docs.microsoft.com/graph/webhooks)
- [Instrucțiuni de limitare](https://docs.microsoft.com/graph/throttling)

**Unde pot găsi mai multe informații despre erori și probleme cunoscute?**

- [Informații despre răspunsul la eroarea Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Probleme cunoscute cu Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Unde pot verifica starea disponibilității și a conectivității serviciului?**

Disponibilitatea serviciului și conectivitatea serviciilor subiacente care pot fi accesate prin intermediul Microsoft Graph pot afecta disponibilitatea generală și performanța Microsoft Graph.

- Pentru starea de sănătate a serviciului Azure Active Directory, Verificați starea **securității + Identity** Services listate în [pagina stare Azure](https://azure.microsoft.com/status/).
- Pentru serviciile Office care contribuie la Microsoft Graph, Verificați starea serviciilor listate în [tabloul de bord Health Service Office](https://portal.office.com/adminportal/home#/servicehealth).

Erorile de autorizare Microsoft Graph pot fi rezultatul câtorva probleme diferite, majoritatea generând o eroare 401 sau 403. De exemplu, următoarele pot duce la erori de autorizare:

- [Fluxuri de acces](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios) incorecte
- [Domenii de permisiune](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) incorect configurate
- Lipsa [consimțământului](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Sfârșitul perioadei de asistență pentru biblioteca de autentificare Azure Active Directory (ADAL) și Azure AD Graph API (AAD Graph)_* _

* * Începând cu 30 iunie, 2020 * *, nu vom mai adăuga caracteristici noi la Monica și Azure AD Graph. Vom continua să oferim asistență tehnică și actualizări de securitate, dar nu vom mai furniza actualizări de caracteristici.

**Începând cu 30 iunie, 2022**, vom încheia asistența pentru monica și Azure AD Graph și nu va mai oferi asistență tehnică sau actualizări de securitate.

Aplicațiile care utilizează monica pe versiunile de sistem de operare existente vor continua să funcționeze după această dată, dar nu vor *primi nicio asistență tehnică sau actualizări de securitate*.

Aplicațiile care utilizează Azure AD Graph după această dată nu mai pot primi răspunsuri de la punctul final Azure AD Graph.

**Migrarea monica**

Vă recomandăm să actualizați la [Biblioteca de autentificare Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), care are cele mai recente caracteristici și actualizări de securitate.

Dacă utilizați aplicațiile Microsoft, știți că Microsoft se află în procesul de migrare a aplicațiilor sale la MSAL până la termenul limită de finalizare a asistenței, asigurându-vă că va beneficia de securitatea în curs de desfășurare și de îmbunătățiri ale caracteristicii MSAL.

1. [Citiți întrebările frecvente despre ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Aflați cum să efectuați migrarea aplicațiilor pe fiecare platformă](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Dacă aveți nevoie de ajutor pentru a înțelege ce aplicații utilizați Monica, vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor și, dacă este cazul, să contactați orice ISV sau furnizori de aplicații. De asemenea, asistența Microsoft vă poate oferi o listă a tuturor aplicațiilor ADAL care nu provin de la Microsoft din entitatea găzduită.

**Migrarea AAD Graph**

Pentru aplicațiile care utilizează Azure AD Graph, urmați ghidul nostru pentru a [migra aplicațiile AZURE AD Graph la Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Lista noastră de verificarea migrării oferă un punct de pornire](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Portalul de înregistrare a aplicațiilor Azure afișează ce aplicații utilizează AAD Graph. Vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor dvs. și, dacă este cazul, să contactați orice furnizor de software independent sau furnizor de aplicații. Asistența Microsoft vă poate oferi, de asemenea, o listă cu utilizarea tuturor grafurilor în entitatea găzduită.
3. Pentru ca aplicația să acceseze date în Microsoft Graph, utilizatorul sau administratorul trebuie să îi acorde permisiunile corecte printr-un proces de consimțământ. [Referințele pentru permisiunile Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) listează permisiunile asociate cu fiecare set principal de API-uri Microsoft Graph. De asemenea, furnizează instrucțiuni despre cum se utilizează permisiunile.
