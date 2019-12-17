---
title: Probleme de performanță-SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068426"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="36fce-102">SharePoint sau OneDrive lent, inaccesibil sau indisponibil pentru mai mulți utilizatori</span><span class="sxs-lookup"><span data-stu-id="36fce-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="36fce-103">SharePoint sau OneDrive poate fi lent, inaccesibil sau indisponibil, sau poate afișa Serviciu indisponibil sau 503 erori, din mai multe motive:</span><span class="sxs-lookup"><span data-stu-id="36fce-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="36fce-104">Dacă site-ul SharePoint sau OneDrive este lent sau întârziat pentru mai mulți utilizatori, poate exista o problemă de serviciu temporar în cazul în care utilizatorii experimenta întârzieri intermitente sau erori de navigare la accesarea site-uri SharePoint sau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="36fce-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="36fce-105">Verificați [tabloul de bord sănătate Service](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) pentru a vedea dacă organizația este afectată.</span><span class="sxs-lookup"><span data-stu-id="36fce-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="36fce-106">Utilizatorii pot primi un *server 503 este ocupat* de eroare atunci când încercați să navigați la site-uri SharePoint sau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="36fce-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="36fce-107">Această eroare poate fi cauzată de limitare în cadrul serviciului SharePoint.</span><span class="sxs-lookup"><span data-stu-id="36fce-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="36fce-108">SharePoint Online utilizează supraîncărcarea pentru a menține performanța optimă și fiabilitatea serviciului SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="36fce-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="36fce-109">Limitare limitează numărul de acțiuni de utilizator sau apeluri simultane (prin script sau cod) pentru a preveni utilizarea excesivă a resurselor.</span><span class="sxs-lookup"><span data-stu-id="36fce-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="36fce-110">Pentru mai multe informații despre limitare a se vedea, [evitați obtinerea limitate sau blocat în SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="36fce-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="36fce-111">Dacă întâmpinați performanțe lente cu un site sau o pagină SharePoint **clasică** sau **modernă** , utilizați [Instrumentul de diagnosticare](https://aka.ms/perftool) a paginilor pentru a analiza paginile.</span><span class="sxs-lookup"><span data-stu-id="36fce-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="36fce-112">Dacă încă vă confruntați cu performanțe lente generale, vă rugăm să revizuiți resursele din partea de jos a acestui articol: [Introducere în reglarea performanței pentru SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="36fce-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  