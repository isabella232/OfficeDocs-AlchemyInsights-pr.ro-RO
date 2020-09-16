---
title: Probleme de performanță-SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771913"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="e1c94-102">SharePoint sau OneDrive este lent, inaccesibil sau indisponibil pentru mai mulți utilizatori</span><span class="sxs-lookup"><span data-stu-id="e1c94-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="e1c94-103">SharePoint sau OneDrive pot fi lente, inaccesibile sau indisponibile sau pot afișa erorile de serviciu indisponibile sau 503, din mai multe motive:</span><span class="sxs-lookup"><span data-stu-id="e1c94-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="e1c94-104">Dacă site-ul SharePoint sau OneDrive este lent sau întârziat pentru mai mulți utilizatori, este posibil să existe o problemă de serviciu temporară în care utilizatorii întâmpină întârzieri intermitente sau erori de navigare atunci când accesează site-uri SharePoint sau conținut OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e1c94-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="e1c94-105">Verificați [tabloul de bord stare servicii](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) pentru a vedea dacă organizația este afectată.</span><span class="sxs-lookup"><span data-stu-id="e1c94-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="e1c94-106">Utilizatorii pot primi un *server 503 este o eroare ocupată* atunci când încercați să navigați la site-uri SharePoint sau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e1c94-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="e1c94-107">Această eroare poate fi cauzată de limitarea în serviciul SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e1c94-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="e1c94-108">SharePoint Online utilizează limitarea pentru a menține performanța optimă și fiabilitatea serviciului SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="e1c94-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="e1c94-109">Limitarea se aplică la numărul de acțiuni de utilizator sau apeluri concurente (după script sau cod), pentru a preveni utilizarea excesivă a resurselor.</span><span class="sxs-lookup"><span data-stu-id="e1c94-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="e1c94-110">Pentru mai multe informații despre limitare, consultați [evitați să fiți accelerat sau blocat în SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="e1c94-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="e1c94-111">Dacă vă confruntați cu o performanță lentă cu un site sau o pagină SharePoint **clasică** sau **modernă** , utilizați [Instrumentul de diagnosticare](https://aka.ms/perftool) a paginilor pentru a analiza paginile.</span><span class="sxs-lookup"><span data-stu-id="e1c94-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="e1c94-112">Dacă încă întâmpinați performanțe generale lente, consultați resursele din partea de jos a acestui articol: [Introducere în ajustarea performanței pentru SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="e1c94-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  