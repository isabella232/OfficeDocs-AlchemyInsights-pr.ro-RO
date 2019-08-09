---
title: Flux de lucru nu este de plecare
ms.author: efrene
author: efrene
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
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270792"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="69472-102">Flux de lucru nu este de plecare</span><span class="sxs-lookup"><span data-stu-id="69472-102">Workflow is not starting</span></span>

- <span data-ttu-id="69472-103">Fluxuri de lucru SharePoint 2010 şi SharePoint 2013 nu incep.</span><span class="sxs-lookup"><span data-stu-id="69472-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="69472-104">În cazul în care nu începe fluxul de lucru, poate fi o problemă temporară de serviciu în cazul în care utilizatorii pot experienţă întârzieri intermitentă cu progresul de flux de lucru.</span><span class="sxs-lookup"><span data-stu-id="69472-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="69472-105">Verifica [Serviciul sănătate tabloul de bord](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) pentru a vedea dacă organizaţia dumneavoastră este afectat.</span><span class="sxs-lookup"><span data-stu-id="69472-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="69472-106">În cazul în care mai mult de 24 de ore au trecut de când aţi văzut prima dată această problemă, vă rugăm să vă un bilet de sprijin.</span><span class="sxs-lookup"><span data-stu-id="69472-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="69472-107">În multe cazuri, lucrăm deja la o soluţie.</span><span class="sxs-lookup"><span data-stu-id="69472-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="69472-108">Vă rugăm să ne dea cel puţin 24 de ore pentru a finaliza o soluţie.</span><span class="sxs-lookup"><span data-stu-id="69472-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="69472-109">Fluxuri de lucru SharePoint 2010 întârziat pe start.</span><span class="sxs-lookup"><span data-stu-id="69472-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="69472-110">Acest lucru se întâmplă în cazul în care fluxul de lucru este declanşată în loturi mari.</span><span class="sxs-lookup"><span data-stu-id="69472-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="69472-111">(de exemplu, când mai multe elemente se adaugă la o dată).</span><span class="sxs-lookup"><span data-stu-id="69472-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="69472-112">Fluxurile de lucru nu sunt concepute pentru a rula în timp real, astfel încât o întârziere este comportamentul de design.</span><span class="sxs-lookup"><span data-stu-id="69472-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="69472-113">În cazul în care fluxul de lucru este complex extensibil obiect Markup Language (XMOL), compilaţie poate fi lent.</span><span class="sxs-lookup"><span data-stu-id="69472-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="69472-114">Verificaţi [acest](https://support.microsoft.com/en-us/kb/3043697) articol.</span><span class="sxs-lookup"><span data-stu-id="69472-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="69472-115">Ar simplifica fluxul de lucru sau redesign-l utilizând tipul de platforma Microsoft SharePoint 2013 de flux de lucru.</span><span class="sxs-lookup"><span data-stu-id="69472-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="69472-116">În cazul în care istoricul de flux de lucru a crescut mare, poate doriţi să purge elementele sau creați o listă nouă de istorie.</span><span class="sxs-lookup"><span data-stu-id="69472-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="69472-117">Mai multe informaţii: [epurare istorie de flux de lucru](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="69472-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="69472-118">Subiecte asociate</span><span class="sxs-lookup"><span data-stu-id="69472-118">Related topics</span></span>
<span data-ttu-id="69472-119">Doriţi să încercaţi Flow Microsoft SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="69472-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="69472-120">Crea fluxul</span><span class="sxs-lookup"><span data-stu-id="69472-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="69472-121">SharePoint şi fluxul</span><span class="sxs-lookup"><span data-stu-id="69472-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


