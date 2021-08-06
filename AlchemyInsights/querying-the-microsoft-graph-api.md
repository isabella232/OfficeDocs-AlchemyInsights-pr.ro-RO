---
title: Interogarea api-ului Microsoft Graph API
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
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923251"
---
# <a name="querying-the-microsoft-graph-api"></a>Interogarea api-ului Microsoft Graph API

Acest subiect se poate aplica și dezvoltatorilor care utilizează în continuare Azure AD Graph API. Cu toate acestea, **se recomandă** ferm să utilizați Microsoft Graph pentru toate scenariile dvs. de gestionare a directorului, identității și accesului.

**Probleme de autentificare sau de autorizare**

- Dacă aplicația  dvs. nu poate obține simboluri pentru a apela Microsoft Graph, alegeți Problemă cu obținerea unui simbol de acces **(autentificare)** categoria Microsoft Graph pentru a obține ajutor și asistență mai specifice în acest subiect.
- Dacă aplicația dvs. primește **401 sau 403** erori **de** autorizare atunci când apelați Microsoft Graph, alegeți categoria Microsoft Graph API Obținere acces refuzat, pentru a obține ajutor și asistență mai specifice cu privire la acest subiect.

**Vreau să utilizez Microsoft Graph, dar nu sunt sigur de unde să încep**

Pentru a afla mai multe despre Microsoft Graph, consultați:

- [Prezentare generală Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Prezentare generală a identității și a gestionării accesului în Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Noțiuni de bază despre construirea Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - testarea API-Graph Microsoft în entitatea găzduită sau într-o entitate găzduită de demonstrație

**Vreau să utilizez Microsoft Graph, dar acceptă API-urile director v1.0 de care am nevoie?**

Microsoft Graph API recomandat pentru gestionarea directoarelor, a identității și a accesului. Cu toate acestea, există încă câteva goluri între ceea ce este posibil în Azure AD Graph și Microsoft Graph. Examinați articolele următoare, care evidențiază cele mai recente diferențe care vă pot ajuta în alegerea dvs.:

- [Diferențele dintre tipurile de resurse, Graph Azure AD și Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Diferențe de proprietate între Azure AD Graph Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Diferențele de metodă dintre Azure AD și Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**When I query the *user* object, many of its properties are missing**

`GET https://graph.microsoft.com/v1.0/users`returnează doar 11 proprietăți, deoarece Microsoft Graph selectează automat un set implicit de proprietăți de *utilizator* de returnat. Dacă aveți nevoie de alte *proprietăți* de utilizator, $select pentru a alege proprietățile de care are nevoie aplicația. Încercați-l mai **întâi în Microsoft Graph Explorer.**

**Unele valori de proprietate de utilizator *sunt nule* chiar dacă știu că sunt setate**

Explicația cea mai probabilă este că aplicația a fost acordată *permisiunii User.ReadBasic.All.* Aceasta permite aplicației să citească un set limitat de proprietăți de utilizator, returnând toate celelalte proprietăți ca nule, chiar dacă au fost setate anterior. Încercați în schimb să acordarea *permisiunii User.Read.All* aplicației.

Pentru mai multe informații, [consultați Permisiunile Graph Microsoft.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**Am probleme cu utilizarea parametrilor de interogare OData pentru a filtra datele din solicitările mele**

Deși Microsoft Graph acceptă o gamă largă de parametri de interogare OData, mulți dintre acești parametri nu sunt complet oferiți de serviciile director (resursele care moștenesc de la *directoryObject)* în Microsoft Graph. Aceleași limitări prezente în Azure AD Graph persistă în majoritatea cazurilor în Microsoft Graph:

1. **Nu se acceptă:**$count, $search valorile $filter *valorile nule* *sau nule*
2. **Nu se acceptă:**$filter proprietăților specifice (consultați subiecte despre resurse despre proprietățile care pot fi filtrate)
3. **Nu se acceptă:** paginare, filtrare și sortare în același timp
4. **Nu se acceptă:** filtrarea după o relație. De exemplu - găsiți toți membrii grupului de inginerie din Regatul Unit.
5. **Asistență parțială:**$orderby pentru *utilizator* (doar displayName și userPrincipalName) și *grup*
6. **Asistență parțială**: $filter (acceptă doar *eq* *,* începe cu *sau* *și*, și , și limitată orice *suport*), $expand (extinderea relațiilor unui singur obiect returnează toate relațiile, dar extinderea unei colecții de relații de obiecte este limitată)

Pentru mai multe informații, [consultați Particularizarea răspunsurilor cu parametri de interogare.](https://docs.microsoft.com/graph/query-parameters)

**Api-ul pe care îl apelez nu funcționează - unde pot să testez mai mult?**

**Microsoft Graph Explorer** - testați API-urile Microsoft Graph din entitatea găzduită sau  dintr-o entitate găzduită de demonstrație și consultați interogările eșantion din Microsoft Graph Explorer.

**Când interog încerc date, pare că primesc din nou un set incomplet de date**

Dacă interogați o colecție (cum ar fi *utilizatori),* Microsoft Graph utilizează limitele de pagină pe partea server, astfel încât rezultatele să fie returnate întotdeauna cu o dimensiune de pagină implicită. Aplicația dvs. ar trebui să se aștepte întotdeauna să pagină prin colecțiile returnate de serviciu.

Pentru mai multe informații, consultați:

- [Cele Graph bune practici Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Paginarea datelor Microsoft Graph din aplicația dvs.](https://docs.microsoft.com/graph/paging)

**Aplicația mea este prea lentă și se amână. Ce îmbunătățiri pot face?**

În funcție de scenariul dvs., există o varietate de opțiuni diferite la dispoziție pentru a face aplicația mai performantă și, în unele cazuri, mai puțin predispusă la reglajul serviciului (atunci când efectuați prea multe apeluri).

Pentru a afla mai multe, consultați:

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
