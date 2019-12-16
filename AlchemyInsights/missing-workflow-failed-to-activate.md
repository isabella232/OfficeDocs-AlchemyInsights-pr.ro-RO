---
title: Flux de lucru lipsă nu a reușit să activați
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 3df1ddc1059c4cd6cc3f9f42dc157d20be79a63a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052625"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="e05ba-102">Flux de lucru lipsă nu a reușit să activați</span><span class="sxs-lookup"><span data-stu-id="e05ba-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="e05ba-103">Într-o colecție de site-ul Microsoft SharePoint, nu puteți adăuga un flux de lucru reutilizabile global (cum ar fi "aprobare-SharePoint 2010") la o listă sau bibliotecă.</span><span class="sxs-lookup"><span data-stu-id="e05ba-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="e05ba-104">Pentru a rezolva această problemă, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="e05ba-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="e05ba-105">Deschideți site-ul rădăcină al colecția de site-uri în SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="e05ba-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="e05ba-106">Sub **obiecte site**, selectați **fluxuri**de lucru.</span><span class="sxs-lookup"><span data-stu-id="e05ba-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="e05ba-107">În secțiunea **nouă** a panglicii **fluxurilor** de lucru, selectați **flux de lucru reutilizabile**.</span><span class="sxs-lookup"><span data-stu-id="e05ba-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="e05ba-108">În formularul **Creare flux de lucru reutilizabile** , introduceți numele \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="e05ba-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="e05ba-109">Pentru **tip de platformă**, faceți clic pe **SharePoint 2010 flux de lucru**, și apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="e05ba-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="e05ba-110">În secțiunea **Salvare** a panglicii **fluxului de lucru** , selectați **Publicare**.</span><span class="sxs-lookup"><span data-stu-id="e05ba-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="e05ba-111">În secțiunea **gestionare** a panglicii **fluxului de lucru** , selectați **Publicare globală**.</span><span class="sxs-lookup"><span data-stu-id="e05ba-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="e05ba-112">În caseta de dialog de confirmare care apare, selectați **OK**.</span><span class="sxs-lookup"><span data-stu-id="e05ba-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="e05ba-113">Într-un browser web, localizați site-ul web rădăcină al colecției de site-uri, apoi accesați **caracteristicile de colecție**site-ul de **Setări** \> site.</span><span class="sxs-lookup"><span data-stu-id="e05ba-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="e05ba-114">Apoi, comutați caracteristica **fluxuri** de lucru:</span><span class="sxs-lookup"><span data-stu-id="e05ba-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="e05ba-115">· Dacă caracteristica este *activată* , faceți clic pe **Dezactivare,** apoi faceți clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="e05ba-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="e05ba-116">· Dacă caracteristica este *dezactivată* , faceți clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="e05ba-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="e05ba-117">Pentru mai multe informații vă rugăm să consultați următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="e05ba-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

