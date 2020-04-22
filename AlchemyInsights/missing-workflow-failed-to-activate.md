---
title: Fluxul de lucru lipsă nu a reușit să se activeze
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762113"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="7e267-102">Fluxul de lucru lipsă nu a reușit să se activeze</span><span class="sxs-lookup"><span data-stu-id="7e267-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="7e267-103">Într-o colecție de site-uri Microsoft SharePoint, nu puteți adăuga un flux de lucru reutilizabil la nivel global (cum ar fi "Aprobare - SharePoint 2010") la o listă sau la o bibliotecă.</span><span class="sxs-lookup"><span data-stu-id="7e267-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="7e267-104">Pentru a rezolva această problemă, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="7e267-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="7e267-105">Deschideți site-ul web rădăcină al colecției de site-uri în SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="7e267-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="7e267-106">Sub **Obiecte site**, selectați Fluxuri de **lucru**.</span><span class="sxs-lookup"><span data-stu-id="7e267-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="7e267-107">În secțiunea **Nou** din panglica **Fluxuri de lucru,** selectați **Flux de lucru reutilizabil**.</span><span class="sxs-lookup"><span data-stu-id="7e267-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="7e267-108">În formularul **Creare flux de lucru reutilizabil,** introduceți numele \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="7e267-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="7e267-109">Pentru **Platformă Tip**, faceți clic pe **Flux de lucru SharePoint 2010**, apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="7e267-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="7e267-110">În secțiunea **Salvare** din panglica **Flux de lucru,** selectați **Publicare**.</span><span class="sxs-lookup"><span data-stu-id="7e267-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="7e267-111">În secțiunea **Gestionare** din panglica Flux de **lucru,** selectați **Publicare globală**.</span><span class="sxs-lookup"><span data-stu-id="7e267-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="7e267-112">În caseta de dialog de confirmare care apare, selectați **OK**.</span><span class="sxs-lookup"><span data-stu-id="7e267-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="7e267-113">Într-un browser web, găsiți site-ul web rădăcină al colecției de site-uri, apoi accesați **Caracteristici colecție de site-uri** **setări** \> site.</span><span class="sxs-lookup"><span data-stu-id="7e267-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="7e267-114">Apoi, comutați caracteristica **Fluxuri de lucru:**</span><span class="sxs-lookup"><span data-stu-id="7e267-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="7e267-115">· Dacă caracteristica este *Activată* , faceți clic pe **Dezactivare,** apoi faceți clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="7e267-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="7e267-116">· Dacă caracteristica este *dezactivată* , faceți clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="7e267-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="7e267-117">Pentru mai multe informații, vă rugăm să consultați următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="7e267-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

