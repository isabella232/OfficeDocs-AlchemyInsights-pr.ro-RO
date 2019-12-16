---
title: Fluxul de lucru nu pornește
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: cf7bd95e9a8f1d0842f0abcf82c758d649e80c0f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049349"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="301df-102">Fluxul de lucru nu pornește</span><span class="sxs-lookup"><span data-stu-id="301df-102">Workflow is not starting</span></span>

- <span data-ttu-id="301df-103">SharePoint 2010 și SharePoint 2013 fluxuri de lucru nu pornesc.</span><span class="sxs-lookup"><span data-stu-id="301df-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="301df-104">Dacă fluxul de lucru nu pornește, este posibil să existe o problemă de serviciu temporară în care utilizatorii pot experimenta întârzieri intermitente cu progresul fluxului de lucru.</span><span class="sxs-lookup"><span data-stu-id="301df-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="301df-105">Verificați [tabloul de bord sănătate Service](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) pentru a vedea dacă organizația este afectată.</span><span class="sxs-lookup"><span data-stu-id="301df-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="301df-106">Dacă au trecut mai mult de 24 de ore de când ați văzut prima dată această problemă, vă rugăm să înregistrați un bilet de suport.</span><span class="sxs-lookup"><span data-stu-id="301df-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="301df-107">În multe cazuri, suntem deja de lucru pe o soluție.</span><span class="sxs-lookup"><span data-stu-id="301df-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="301df-108">Vă rugăm să ne acordați cel puțin 24 de ore pentru a finaliza o soluție.</span><span class="sxs-lookup"><span data-stu-id="301df-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="301df-109">Fluxurile de lucru SharePoint 2010 întârziate la pornire.</span><span class="sxs-lookup"><span data-stu-id="301df-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="301df-110">Acest lucru se întâmplă dacă fluxul de lucru este declanșat în loturi mari.</span><span class="sxs-lookup"><span data-stu-id="301df-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="301df-111">(de exemplu, atunci când mai multe elemente sunt adăugate la o dată).</span><span class="sxs-lookup"><span data-stu-id="301df-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="301df-112">Fluxurile de lucru nu sunt proiectate să ruleze în timp real, astfel încât o întârziere este un comportament de proiectare.</span><span class="sxs-lookup"><span data-stu-id="301df-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="301df-113">Dacă fluxul de lucru este complex extensibil obiect Markup Language (XMOL), compilarea poate fi lentă.</span><span class="sxs-lookup"><span data-stu-id="301df-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="301df-114">Verificați [acest](https://support.microsoft.com//kb/3043697) articol.</span><span class="sxs-lookup"><span data-stu-id="301df-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="301df-115">Trebuie să Simplificați fluxul de lucru sau să îl reproiectați utilizând tipul platformei Microsoft SharePoint 2013 Workflow.</span><span class="sxs-lookup"><span data-stu-id="301df-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="301df-116">Dacă Istoricul fluxului de lucru a crescut mare, este posibil să doriți să curățați elementele sau să creați o nouă listă de istoric.</span><span class="sxs-lookup"><span data-stu-id="301df-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="301df-117">Mai multe informații: [golirea istoricului fluxului de lucru](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="301df-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="301df-118">Subiecte asociate</span><span class="sxs-lookup"><span data-stu-id="301df-118">Related topics</span></span>
<span data-ttu-id="301df-119">Doriți să încercați Microsoft Flow în SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="301df-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="301df-120">Creare flux</span><span class="sxs-lookup"><span data-stu-id="301df-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="301df-121">SharePoint și flux</span><span class="sxs-lookup"><span data-stu-id="301df-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


