---
title: Fluxul de lucru nu porni
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403755"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="d1c6a-102">Fluxul de lucru nu porni</span><span class="sxs-lookup"><span data-stu-id="d1c6a-102">Workflow is not starting</span></span>

- <span data-ttu-id="d1c6a-103">Fluxurile de lucru SharePoint 2010 și SharePoint 2013 nu rulează.</span><span class="sxs-lookup"><span data-stu-id="d1c6a-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="d1c6a-104">Dacă fluxul dvs. de lucru nu începe, poate exista o problemă temporară de serviciu în care utilizatorii se pot experimenta întârzieri intermitente în progresul fluxului de lucru.</span><span class="sxs-lookup"><span data-stu-id="d1c6a-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="d1c6a-105">Verificați tabloul [de bord cu starea](https://admin.microsoft.com/AdminPortal/Home/servicehealth) serviciilor pentru a vedea dacă organizația dvs. este afectat.</span><span class="sxs-lookup"><span data-stu-id="d1c6a-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="d1c6a-106">Dacă au trecut mai mult de 24 de ore de când ați văzut prima dată această problemă, vă rugăm să introduceți în jurnal un tichet de asistență.</span><span class="sxs-lookup"><span data-stu-id="d1c6a-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="d1c6a-107">În multe cazuri, lucrăm deja la o soluție.</span><span class="sxs-lookup"><span data-stu-id="d1c6a-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="d1c6a-108">Acordați-ne cel puțin 24 de ore pentru a finaliza o soluție.</span><span class="sxs-lookup"><span data-stu-id="d1c6a-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="d1c6a-109">Fluxurile de lucru SharePoint 2010 au întârziat la pornire.</span><span class="sxs-lookup"><span data-stu-id="d1c6a-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="d1c6a-110">Acest lucru se întâmplă dacă fluxul de lucru este declanșat în grupuri mari.</span><span class="sxs-lookup"><span data-stu-id="d1c6a-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="d1c6a-111">(de exemplu, când se adaugă mai multe elemente simultan).</span><span class="sxs-lookup"><span data-stu-id="d1c6a-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="d1c6a-112">Fluxurile de lucru nu sunt proiectate pentru a rula în timp real, astfel că o întârziere este un comportament prin proiectare.</span><span class="sxs-lookup"><span data-stu-id="d1c6a-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="d1c6a-113">Dacă Fluxul de lucru este un limbaj X SCURT (Extensible Object Markup Language), compilarea poate fi lentă.</span><span class="sxs-lookup"><span data-stu-id="d1c6a-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="d1c6a-114">Consultați [acest](https://support.microsoft.com//kb/3043697) articol.</span><span class="sxs-lookup"><span data-stu-id="d1c6a-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="d1c6a-115">Trebuie să simplificați fluxul de lucru sau să-l reproiectați utilizând tipul de platformă de flux de lucru Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="d1c6a-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="d1c6a-116">Dacă istoricul fluxului de lucru s-a dezvoltat, se poate să doriți să goliți elementele sau să creați o nouă listă de istoric.</span><span class="sxs-lookup"><span data-stu-id="d1c6a-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="d1c6a-117">Mai multe informații: [Goliți istoricul fluxului de lucru](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="d1c6a-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="d1c6a-118">Subiecte asociate</span><span class="sxs-lookup"><span data-stu-id="d1c6a-118">Related topics</span></span>
<span data-ttu-id="d1c6a-119">Doriți să încercați Microsoft Flow în SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="d1c6a-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="d1c6a-120">Create Flow</span><span class="sxs-lookup"><span data-stu-id="d1c6a-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="d1c6a-121">SharePoint și Flow</span><span class="sxs-lookup"><span data-stu-id="d1c6a-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
