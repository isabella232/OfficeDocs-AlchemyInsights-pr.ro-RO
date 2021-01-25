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
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="566ed-102">Interogarea API-ului Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="566ed-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="566ed-103">Acest subiect se poate aplica și pentru dezvoltatori care utilizează încă Azure AD Graph API.</span><span class="sxs-lookup"><span data-stu-id="566ed-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="566ed-104">Cu toate acestea, se recomandă **insistent** să utilizați Microsoft Graph pentru toate scenariile de gestionare a directorului, identității și Access.</span><span class="sxs-lookup"><span data-stu-id="566ed-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="566ed-105">**Probleme de autentificare sau de autorizare**</span><span class="sxs-lookup"><span data-stu-id="566ed-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="566ed-106">Dacă aplicația **nu reușește să obțină tokenuri** pentru a apela Microsoft Graph, alegeți **problema cu obținerea unei categorii de simboluri Access (autentificare)** Microsoft Graph pentru a obține ajutor și asistență specifice pentru acest subiect.</span><span class="sxs-lookup"><span data-stu-id="566ed-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="566ed-107">În cazul în care aplicația **primește erori de autorizare 401 sau 403** atunci când apelare Microsoft Graph, alegeți categoria **Obțineți o eroare Access Denied (autorizare)** Microsoft Graph API pentru a obține ajutor și asistență specifice în acest articol.</span><span class="sxs-lookup"><span data-stu-id="566ed-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="566ed-108">**Doresc să utilizez Microsoft Graph, dar nu sunt sigur de unde să încep**</span><span class="sxs-lookup"><span data-stu-id="566ed-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="566ed-109">Pentru a afla mai multe despre Microsoft Graph, consultați:</span><span class="sxs-lookup"><span data-stu-id="566ed-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="566ed-110">Prezentare generală a Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="566ed-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="566ed-111">Prezentare generală a identității și gestionării accesului în Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="566ed-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="566ed-112">Introducere în construirea aplicațiilor Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="566ed-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="566ed-113">**Microsoft Graph Explorer** -testați API-uri Microsoft Graph în entitatea găzduită sau într-o entitate găzduită demo</span><span class="sxs-lookup"><span data-stu-id="566ed-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="566ed-114">**Doresc să utilizez Microsoft Graph, dar acceptă API-urile de directoare v 1.0 de care am nevoie?**</span><span class="sxs-lookup"><span data-stu-id="566ed-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="566ed-115">Microsoft Graph este API-ul recomandat pentru directorul, identitatea și gestionarea accesului.</span><span class="sxs-lookup"><span data-stu-id="566ed-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="566ed-116">Cu toate acestea, există încă câteva lacune între ceea ce este posibil în Azure AD Graph și Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="566ed-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="566ed-117">Revizuiți următoarele articole, care evidențiază cele mai recente diferențe de asistență în alegerea dvs.:</span><span class="sxs-lookup"><span data-stu-id="566ed-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="566ed-118">Diferențele de tip de resursă între Azure AD Graph și Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="566ed-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="566ed-119">Diferențe de proprietăți între Azure AD Graph și Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="566ed-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="566ed-120">Diferențe de metodă între Azure AD și Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="566ed-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="566ed-121">**Când se interoghează obiectul *utilizator* , multe dintre proprietățile sale lipsesc**</span><span class="sxs-lookup"><span data-stu-id="566ed-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="566ed-122">`GET https://graph.microsoft.com/v1.0/users` returnează doar 11 proprietăți, deoarece Microsoft Graph auto-selectează un set implicit de proprietăți de *utilizator* de returnat.</span><span class="sxs-lookup"><span data-stu-id="566ed-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="566ed-123">Dacă aveți nevoie de alte proprietăți de *utilizator* , utilizați $Select pentru a alege proprietățile necesare aplicației.</span><span class="sxs-lookup"><span data-stu-id="566ed-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="566ed-124">Încercați mai întâi în **Microsoft Graph Explorer** .</span><span class="sxs-lookup"><span data-stu-id="566ed-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="566ed-125">**Unele valori ale proprietății de utilizator sunt *nule* , chiar dacă știu că sunt setate**</span><span class="sxs-lookup"><span data-stu-id="566ed-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="566ed-126">Explicația cea mai probabilă este că aplicației i s-a acordat *utilizatorului. ReadBasic. All* permission.</span><span class="sxs-lookup"><span data-stu-id="566ed-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="566ed-127">Acest lucru permite aplicației să citească un set limitat de proprietăți de utilizator, returnând toate celelalte proprietăți ca NULL chiar dacă au fost setate anterior.</span><span class="sxs-lookup"><span data-stu-id="566ed-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="566ed-128">Încercați să acordați *utilizatorului aplicației. citiți. toate* permisiunile în schimb.</span><span class="sxs-lookup"><span data-stu-id="566ed-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="566ed-129">Pentru mai multe informații, consultați [permisiunile de utilizator Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="566ed-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="566ed-130">**Am probleme cu utilizarea parametrilor de interogare OData pentru a filtra datele în solicitările mele**</span><span class="sxs-lookup"><span data-stu-id="566ed-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="566ed-131">În timp ce Microsoft Graph acceptă o gamă largă de parametri de interogare OData, mulți dintre acești parametri nu sunt acceptați pe deplin de serviciile de director (resursele care moștenesc din *directoryObject*) în Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="566ed-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="566ed-132">Aceleași limite care au fost prezente în Azure AD Graph persistă în cea mai mare parte din Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="566ed-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="566ed-133">**Neacceptat**: $count, $search și *$Filter la valori Null sau* *NOT NULL*</span><span class="sxs-lookup"><span data-stu-id="566ed-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="566ed-134">**Neacceptat**: $Filter în anumite proprietăți (consultați subiecte de resurse pe care se pot filtra proprietățile)</span><span class="sxs-lookup"><span data-stu-id="566ed-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="566ed-135">**Neacceptat**: paginarea, filtrarea și sortarea în același timp</span><span class="sxs-lookup"><span data-stu-id="566ed-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="566ed-136">**Neacceptat**: filtrarea într-o relație.</span><span class="sxs-lookup"><span data-stu-id="566ed-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="566ed-137">De exemplu, găsiți toți membrii grupului de inginerie care se află în Marea Britanie.</span><span class="sxs-lookup"><span data-stu-id="566ed-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="566ed-138">**Suport parțial**: $orderby pentru *utilizator* (numai pentru DisplayName și UserPrincipalName) și *grup*</span><span class="sxs-lookup"><span data-stu-id="566ed-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="566ed-139">**Suport parțial**: $Filter (acceptă doar suport pentru *EQ*,  *Startswith* sau *, și și* limitat *),*$Expand (extinderea relațiilor unui singur obiect returnează toate relațiile, dar extinderea unei colecții de relații de obiecte este limitată)</span><span class="sxs-lookup"><span data-stu-id="566ed-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="566ed-140">Pentru mai multe informații, consultați [Particularizarea răspunsurilor cu parametri de interogare](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="566ed-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="566ed-141">**API-ul pe care îl sun nu funcționează-unde pot face mai multe teste?**</span><span class="sxs-lookup"><span data-stu-id="566ed-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="566ed-142">**Microsoft Graph Explorer** -testați API-uri Microsoft Graph în entitatea găzduită sau într-o entitate găzduită demo și consultați și **interogările eșantion** din Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="566ed-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="566ed-143">**Când fac o interogare pentru date, se pare că primesc un set de date incomplete înapoi**</span><span class="sxs-lookup"><span data-stu-id="566ed-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="566ed-144">Dacă interogați o colecție (cum ar fi *utilizatori*), Microsoft Graph utilizează limite de pagină pe partea server, astfel încât rezultatele să fie întotdeauna returnate cu o dimensiune implicită de pagină.</span><span class="sxs-lookup"><span data-stu-id="566ed-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="566ed-145">Aplicația trebuie să se aștepte întotdeauna la pagina prin colecții returnate de la serviciu.</span><span class="sxs-lookup"><span data-stu-id="566ed-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="566ed-146">Pentru mai multe informații, consultați:</span><span class="sxs-lookup"><span data-stu-id="566ed-146">For more information, see:</span></span>

- [<span data-ttu-id="566ed-147">Cele mai bune practici Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="566ed-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="566ed-148">Paginarea datelor Microsoft Graph în aplicația dvs.</span><span class="sxs-lookup"><span data-stu-id="566ed-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="566ed-149">**Aplicația mea este prea lentă și, de asemenea, este accelerat. Ce îmbunătățiri pot să fac?**</span><span class="sxs-lookup"><span data-stu-id="566ed-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="566ed-150">În funcție de scenariul dvs., există o varietate de opțiuni diferite la dispoziție pentru a face aplicația mai performantă și, în unele cazuri, mai puțin predispus la a fi accelerat de serviciu (atunci când efectuați prea multe apeluri).</span><span class="sxs-lookup"><span data-stu-id="566ed-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="566ed-151">Pentru a afla mai multe, consultați:</span><span class="sxs-lookup"><span data-stu-id="566ed-151">To learn more, see:</span></span>

- [<span data-ttu-id="566ed-152">Cele mai bune practici Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="566ed-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="566ed-153">Solicitări de grupare</span><span class="sxs-lookup"><span data-stu-id="566ed-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="566ed-154">Urmărirea modificărilor prin Delta Query</span><span class="sxs-lookup"><span data-stu-id="566ed-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="566ed-155">Fiți notificat de modificări prin intermediul cârligelor</span><span class="sxs-lookup"><span data-stu-id="566ed-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="566ed-156">Instrucțiuni de limitare</span><span class="sxs-lookup"><span data-stu-id="566ed-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="566ed-157">**Unde pot găsi mai multe informații despre erori și probleme cunoscute?**</span><span class="sxs-lookup"><span data-stu-id="566ed-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="566ed-158">Informații despre răspunsul la eroarea Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="566ed-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="566ed-159">Probleme cunoscute cu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="566ed-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="566ed-160">**Unde pot verifica starea disponibilității și a conectivității serviciului?**</span><span class="sxs-lookup"><span data-stu-id="566ed-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="566ed-161">Disponibilitatea serviciului și conectivitatea serviciilor subiacente care pot fi accesate prin intermediul Microsoft Graph pot afecta disponibilitatea generală și performanța Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="566ed-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="566ed-162">Pentru starea de sănătate a serviciului Azure Active Directory, Verificați starea **securității + Identity** Services listate în [pagina stare Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="566ed-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="566ed-163">Pentru serviciile Office care contribuie la Microsoft Graph, Verificați starea serviciilor listate în [tabloul de bord Health Service Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="566ed-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
