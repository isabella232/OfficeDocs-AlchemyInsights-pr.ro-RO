---
title: Fluxul de lucru nu pornește
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794779"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="d992c-102">Fluxul de lucru nu pornește</span><span class="sxs-lookup"><span data-stu-id="d992c-102">Workflow is not starting</span></span>

- <span data-ttu-id="d992c-103">Fluxurile de lucru SharePoint 2010 și SharePoint 2013 nu pornește.</span><span class="sxs-lookup"><span data-stu-id="d992c-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="d992c-104">Dacă fluxul de lucru nu pornește, este posibil să existe o problemă de serviciu temporară, în care utilizatorii pot avea întârzieri intermitente cu progresul fluxului de lucru.</span><span class="sxs-lookup"><span data-stu-id="d992c-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="d992c-105">Verificați [tabloul de bord stare servicii](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) pentru a vedea dacă organizația este afectată.</span><span class="sxs-lookup"><span data-stu-id="d992c-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="d992c-106">Dacă au trecut mai mult de 24 de ore de când ați văzut prima dată această problemă, vă rugăm să înregistrați un tichet de asistență.</span><span class="sxs-lookup"><span data-stu-id="d992c-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="d992c-107">În multe cazuri, lucrăm deja la o soluție.</span><span class="sxs-lookup"><span data-stu-id="d992c-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="d992c-108">Vă rugăm să ne dați cel puțin 24 de ore pentru a finaliza o soluție.</span><span class="sxs-lookup"><span data-stu-id="d992c-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="d992c-109">Fluxurile de lucru SharePoint 2010 au întârziat la pornire.</span><span class="sxs-lookup"><span data-stu-id="d992c-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="d992c-110">Acest lucru se întâmplă dacă fluxul de lucru este declanșat în grupuri mari.</span><span class="sxs-lookup"><span data-stu-id="d992c-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="d992c-111">(de exemplu, atunci când sunt adăugate mai multe elemente în același timp).</span><span class="sxs-lookup"><span data-stu-id="d992c-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="d992c-112">Fluxurile de lucru nu sunt proiectate să ruleze în timp real, astfel încât o întârziere să fie un comportament de proiectare.</span><span class="sxs-lookup"><span data-stu-id="d992c-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="d992c-113">Dacă fluxul de lucru este complex Extensible Object Markup Language (XMOL), compilarea poate fi lentă.</span><span class="sxs-lookup"><span data-stu-id="d992c-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="d992c-114">Consultați [acest](https://support.microsoft.com//kb/3043697) articol.</span><span class="sxs-lookup"><span data-stu-id="d992c-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="d992c-115">Trebuie să Simplificați fluxul de lucru sau să îl reproiectați utilizând tipul de platformă flux de lucru Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="d992c-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="d992c-116">Dacă Istoricul fluxului de lucru s-a extins, se recomandă să goliți elementele sau să creați o listă de istoric nou.</span><span class="sxs-lookup"><span data-stu-id="d992c-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="d992c-117">Mai multe informații: [golirea istoricului fluxului de lucru](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="d992c-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="d992c-118">Subiecte asociate</span><span class="sxs-lookup"><span data-stu-id="d992c-118">Related topics</span></span>
<span data-ttu-id="d992c-119">Doriți să încercați Microsoft Flow în SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="d992c-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="d992c-120">Crearea fluxului</span><span class="sxs-lookup"><span data-stu-id="d992c-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="d992c-121">SharePoint și fluxul</span><span class="sxs-lookup"><span data-stu-id="d992c-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


