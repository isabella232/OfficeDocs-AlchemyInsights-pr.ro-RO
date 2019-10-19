---
title: Flux de lucru lipsă nu a reușit să activați
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36753808"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="f76ff-102">Flux de lucru lipsă nu a reușit să activați</span><span class="sxs-lookup"><span data-stu-id="f76ff-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="f76ff-103">Într-o colecție de site-ul Microsoft SharePoint, nu puteți adăuga un flux de lucru reutilizabile global (cum ar fi "aprobare-SharePoint 2010") la o listă sau bibliotecă.</span><span class="sxs-lookup"><span data-stu-id="f76ff-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="f76ff-104">Pentru a rezolva această problemă, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="f76ff-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="f76ff-105">Deschideți site-ul rădăcină al colecția de site-uri în SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="f76ff-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="f76ff-106">Sub **obiecte site**, selectați **fluxuri**de lucru.</span><span class="sxs-lookup"><span data-stu-id="f76ff-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="f76ff-107">În secțiunea **nouă** a panglicii **fluxurilor** de lucru, selectați **flux de lucru reutilizabile**.</span><span class="sxs-lookup"><span data-stu-id="f76ff-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="f76ff-108">În formularul **Creare flux de lucru reutilizabile** , introduceți numele \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="f76ff-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="f76ff-109">Pentru **tip de platformă**, faceți clic pe **SharePoint 2010 flux de lucru**, și apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="f76ff-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="f76ff-110">În secțiunea **Salvare** a panglicii **fluxului de lucru** , selectați **Publicare**.</span><span class="sxs-lookup"><span data-stu-id="f76ff-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="f76ff-111">În secțiunea **gestionare** a panglicii **fluxului de lucru** , selectați **Publicare globală**.</span><span class="sxs-lookup"><span data-stu-id="f76ff-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="f76ff-112">În caseta de dialog de confirmare care apare, selectați **OK**.</span><span class="sxs-lookup"><span data-stu-id="f76ff-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="f76ff-113">Într-un browser web, localizați site-ul web rădăcină al colecției de site-uri, apoi accesați **caracteristicile de colecție**site-ul de **Setări** \> site.</span><span class="sxs-lookup"><span data-stu-id="f76ff-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="f76ff-114">Apoi, comutați caracteristica **fluxuri** de lucru:</span><span class="sxs-lookup"><span data-stu-id="f76ff-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="f76ff-115">· Dacă caracteristica este *activată* , faceți clic pe **Dezactivare,** apoi faceți clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="f76ff-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="f76ff-116">· Dacă caracteristica este *dezactivată* , faceți clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="f76ff-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="f76ff-117">Pentru mai multe informații vă rugăm să consultați următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="f76ff-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

