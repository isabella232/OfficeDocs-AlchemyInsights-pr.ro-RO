---
title: Imposibil de adăugat 2010 aprobare flux de lucru
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049565"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="62b4f-102">Imposibil de adăugat 2010 aprobare flux de lucru</span><span class="sxs-lookup"><span data-stu-id="62b4f-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="62b4f-103">Într-o colecție de site-ul Microsoft SharePoint, nu puteți adăuga un flux de lucru reutilizabile global (cum ar fi "aprobare-SharePoint 2010") la o listă sau bibliotecă.</span><span class="sxs-lookup"><span data-stu-id="62b4f-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="62b4f-104">Pentru a rezolva această problemă, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="62b4f-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="62b4f-105">Deschideți site-ul rădăcină al colecția de site-uri în SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="62b4f-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="62b4f-106">Sub **obiecte site**, selectați **fluxuri**de lucru.</span><span class="sxs-lookup"><span data-stu-id="62b4f-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="62b4f-107">În secțiunea **nouă** a panglicii **fluxurilor** de lucru, selectați **flux de lucru reutilizabile**.</span><span class="sxs-lookup"><span data-stu-id="62b4f-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="62b4f-108">În formularul **Creare flux de lucru reutilizabile** , introduceți numele \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="62b4f-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="62b4f-109">Pentru **tip de platformă**, faceți clic pe **SharePoint 2010 flux de lucru**, și apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="62b4f-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="62b4f-110">În secțiunea **Salvare** a panglicii **fluxului de lucru** , selectați **Publicare**.</span><span class="sxs-lookup"><span data-stu-id="62b4f-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="62b4f-111">În secțiunea **gestionare** a panglicii **fluxului de lucru** , selectați **Publicare globală**.</span><span class="sxs-lookup"><span data-stu-id="62b4f-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="62b4f-112">În caseta de dialog de confirmare care apare, selectați **OK**.</span><span class="sxs-lookup"><span data-stu-id="62b4f-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="62b4f-113">Într-un browser web, localizați site-ul web rădăcină al colecției de site-uri, apoi accesați **caracteristicile de colecție**site-ul de **Setări** \> site.</span><span class="sxs-lookup"><span data-stu-id="62b4f-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="62b4f-114">Comutați caracteristica **fluxuri** de lucru:</span><span class="sxs-lookup"><span data-stu-id="62b4f-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="62b4f-115">· Dacă caracteristica este *activată* , faceți clic pe **Dezactivare,** apoi faceți clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="62b4f-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="62b4f-116">· Dacă caracteristica este *dezactivată* , faceți clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="62b4f-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="62b4f-117">Pentru mai multe informații vă rugăm să consultați următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="62b4f-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

