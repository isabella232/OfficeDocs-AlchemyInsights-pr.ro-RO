---
title: Interogarea API-ului Microsoft Graph
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974683"
---
# <a name="querying-the-microsoft-graph-api"></a>Interogarea API-ului Microsoft Graph

Acest subiect se poate aplica și pentru dezvoltatori care utilizează încă Azure AD Graph API. Cu toate acestea, se recomandă **insistent** să utilizați Microsoft Graph pentru toate scenariile de gestionare a directorului, identității și Access.

**Probleme de autentificare sau de autorizare**

- Dacă aplicația **nu reușește să obțină tokenuri** pentru a apela Microsoft Graph, alegeți **problema cu obținerea unei categorii de simboluri Access (autentificare)** Microsoft Graph pentru a obține ajutor și asistență specifice pentru acest subiect.
- În cazul în care aplicația **primește erori de autorizare 401 sau 403** atunci când apelare Microsoft Graph, alegeți categoria **Obțineți o eroare Access Denied (autorizare)** Microsoft Graph API pentru a obține ajutor și asistență specifice în acest articol.

**Doresc să utilizez Microsoft Graph, dar nu sunt sigur de unde să încep**

Pentru a afla mai multe despre Microsoft Graph, consultați:

- [Prezentare generală a Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Prezentare generală a identității și gestionării accesului în Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Introducere în construirea aplicațiilor Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** -testați API-uri Microsoft Graph în entitatea găzduită sau într-o entitate găzduită demo

**Doresc să utilizez Microsoft Graph, dar acceptă API-urile de directoare v 1.0 de care am nevoie?**

Microsoft Graph este API-ul recomandat pentru directorul, identitatea și gestionarea accesului. Cu toate acestea, există încă câteva lacune între ceea ce este posibil în Azure AD Graph și Microsoft Graph. Revizuiți următoarele articole, care evidențiază cele mai recente diferențe de asistență în alegerea dvs.:

- [Diferențele de tip de resursă între Azure AD Graph și Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Diferențe de proprietăți între Azure AD Graph și Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Diferențe de metodă între Azure AD și Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Când se interoghează obiectul *utilizator* , multe dintre proprietățile sale lipsesc**

`GET https://graph.microsoft.com/v1.0/users` returnează doar 11 proprietăți, deoarece Microsoft Graph auto-selectează un set implicit de proprietăți de *utilizator* de returnat. Dacă aveți nevoie de alte proprietăți de *utilizator* , utilizați $Select pentru a alege proprietățile necesare aplicației. Încercați mai întâi în **Microsoft Graph Explorer** .

**Unele valori ale proprietății de utilizator sunt *nule* , chiar dacă știu că sunt setate**

Explicația cea mai probabilă este că aplicației i s-a acordat *utilizatorului. ReadBasic. All* permission. Acest lucru permite aplicației să citească un set limitat de proprietăți de utilizator, returnând toate celelalte proprietăți ca NULL chiar dacă au fost setate anterior. Încercați să acordați *utilizatorului aplicației. citiți. toate* permisiunile în schimb.

Pentru mai multe informații, consultați [permisiunile de utilizator Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Am probleme cu utilizarea parametrilor de interogare OData pentru a filtra datele în solicitările mele**

În timp ce Microsoft Graph acceptă o gamă largă de parametri de interogare OData, mulți dintre acești parametri nu sunt acceptați pe deplin de serviciile de director (resursele care moștenesc din *directoryObject*) în Microsoft Graph. Aceleași limite care au fost prezente în Azure AD Graph persistă în cea mai mare parte din Microsoft Graph:

1. **Neacceptat**: $count, $search și *$Filter la valori Null sau* *NOT NULL*
2. **Neacceptat**: $Filter în anumite proprietăți (consultați subiecte de resurse pe care se pot filtra proprietățile)
3. **Neacceptat**: paginarea, filtrarea și sortarea în același timp
4. **Neacceptat**: filtrarea într-o relație. De exemplu, găsiți toți membrii grupului de inginerie care se află în Marea Britanie.
5. **Suport parțial**: $orderby pentru *utilizator* (numai pentru DisplayName și UserPrincipalName) și *grup*
6. **Suport parțial**: $Filter (acceptă doar suport pentru *EQ*,  *Startswith* sau *, și și* limitat *),*$Expand (extinderea relațiilor unui singur obiect returnează toate relațiile, dar extinderea unei colecții de relații de obiecte este limitată)

Pentru mai multe informații, consultați [Particularizarea răspunsurilor cu parametri de interogare](https://docs.microsoft.com/graph/query-parameters).

**API-ul pe care îl sun nu funcționează-unde pot face mai multe teste?**

**Microsoft Graph Explorer** -testați API-uri Microsoft Graph în entitatea găzduită sau într-o entitate găzduită demo și consultați și **interogările eșantion** din Microsoft Graph Explorer.

**Când fac o interogare pentru date, se pare că primesc un set de date incomplete înapoi**

Dacă interogați o colecție (cum ar fi *utilizatori*), Microsoft Graph utilizează limite de pagină pe partea server, astfel încât rezultatele să fie întotdeauna returnate cu o dimensiune implicită de pagină. Aplicația trebuie să se aștepte întotdeauna la pagina prin colecții returnate de la serviciu.

Pentru mai multe informații, consultați:

- [Cele mai bune practici Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Paginarea datelor Microsoft Graph în aplicația dvs.](https://docs.microsoft.com/graph/paging)

**Aplicația mea este prea lentă și, de asemenea, este accelerat. Ce îmbunătățiri pot să fac?**

În funcție de scenariul dvs., există o varietate de opțiuni diferite la dispoziție pentru a face aplicația mai performantă și, în unele cazuri, mai puțin predispus la a fi accelerat de serviciu (atunci când efectuați prea multe apeluri).

Pentru a afla mai multe, consultați:

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
