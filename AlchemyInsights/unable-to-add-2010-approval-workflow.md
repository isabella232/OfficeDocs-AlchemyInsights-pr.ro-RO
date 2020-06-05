---
title: Imposibil de adăugat fluxul de lucru de aprobare 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582859"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="c8a68-102">Imposibil de adăugat fluxul de lucru de aprobare 2010</span><span class="sxs-lookup"><span data-stu-id="c8a68-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="c8a68-103">Într-o colecție de site-uri Microsoft SharePoint, nu puteți adăuga un flux de lucru reutilizabil la nivel global (cum ar fi "Aprobare - SharePoint 2010") la o listă sau la o bibliotecă.</span><span class="sxs-lookup"><span data-stu-id="c8a68-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="c8a68-104">Pentru a rezolva această problemă, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="c8a68-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="c8a68-105">Deschideți site-ul web rădăcină al colecției de site-uri în SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="c8a68-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="c8a68-106">Sub **Obiecte site**, selectați Fluxuri de **lucru**.</span><span class="sxs-lookup"><span data-stu-id="c8a68-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="c8a68-107">În secțiunea **Nou** din panglica **Fluxuri de lucru,** selectați **Flux de lucru reutilizabil**.</span><span class="sxs-lookup"><span data-stu-id="c8a68-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="c8a68-108">În formularul **Creare flux de lucru reutilizabil,** introduceți numele \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="c8a68-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="c8a68-109">Pentru **Platformă Tip**, faceți clic pe **Flux de lucru SharePoint 2010**, apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="c8a68-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="c8a68-110">În secțiunea **Salvare** din panglica **Flux de lucru,** selectați **Publicare**.</span><span class="sxs-lookup"><span data-stu-id="c8a68-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="c8a68-111">În secțiunea **Gestionare** din panglica Flux de **lucru,** selectați **Publicare globală**.</span><span class="sxs-lookup"><span data-stu-id="c8a68-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="c8a68-112">În caseta de dialog de confirmare care apare, selectați **OK**.</span><span class="sxs-lookup"><span data-stu-id="c8a68-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="c8a68-113">Într-un browser web, găsiți site-ul web rădăcină al colecției de site-uri, apoi accesați Caracteristici colecție de **Site Settings** \> **site-uri**setări site.</span><span class="sxs-lookup"><span data-stu-id="c8a68-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="c8a68-114">Comutați caracteristica **Fluxuri de lucru:**</span><span class="sxs-lookup"><span data-stu-id="c8a68-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="c8a68-115">· Dacă caracteristica este *Activată* , faceți clic pe **Dezactivare,** apoi faceți clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="c8a68-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="c8a68-116">· Dacă caracteristica este *dezactivată* , faceți clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="c8a68-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="c8a68-117">Pentru mai multe informații, vă rugăm să consultați următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="c8a68-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

