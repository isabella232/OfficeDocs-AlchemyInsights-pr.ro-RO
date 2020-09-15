---
title: Nu se poate adăuga un flux de lucru aprobare 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699747"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="0e3ba-102">Nu se poate adăuga un flux de lucru aprobare 2010</span><span class="sxs-lookup"><span data-stu-id="0e3ba-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="0e3ba-103">Într-o colecție de site-uri Microsoft SharePoint, nu puteți adăuga un flux de lucru reutilizabil global (cum ar fi "aprobare-SharePoint 2010") într-o listă sau o bibliotecă.</span><span class="sxs-lookup"><span data-stu-id="0e3ba-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="0e3ba-104">Pentru a rezolva această problemă, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="0e3ba-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="0e3ba-105">Deschideți site-ul web rădăcină al colecției de site-uri în SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="0e3ba-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="0e3ba-106">Sub **obiecte site**, selectați **fluxuri de lucru**.</span><span class="sxs-lookup"><span data-stu-id="0e3ba-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="0e3ba-107">În secțiunea **nouă** a panglicii **fluxuri de lucru** , selectați **flux de lucru reutilizabil**.</span><span class="sxs-lookup"><span data-stu-id="0e3ba-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="0e3ba-108">În formularul **Creați un flux de lucru reutilizabil** , introduceți numele \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="0e3ba-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="0e3ba-109">Pentru **tip platformă**, faceți clic pe **flux de lucru SharePoint 2010**, apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="0e3ba-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="0e3ba-110">În secțiunea **Salvare** a panglicii **fluxului de lucru** , selectați **Publicare**.</span><span class="sxs-lookup"><span data-stu-id="0e3ba-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="0e3ba-111">În secțiunea **gestionare** a panglicii **fluxului de lucru** , selectați **Publicare la nivel global**.</span><span class="sxs-lookup"><span data-stu-id="0e3ba-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="0e3ba-112">În caseta de dialog de confirmare care apare, selectați **OK**.</span><span class="sxs-lookup"><span data-stu-id="0e3ba-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="0e3ba-113">Într-un browser web, găsiți site-ul web rădăcină al colecției de site **Site Settings** -uri, apoi accesați \> **caracteristicile colecției**site-ului setări site.</span><span class="sxs-lookup"><span data-stu-id="0e3ba-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="0e3ba-114">Comutați caracteristica **fluxuri de lucru** :</span><span class="sxs-lookup"><span data-stu-id="0e3ba-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="0e3ba-115">· Dacă caracteristica este  *activată*  , faceți clic pe Dezactivare **,** apoi faceți clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="0e3ba-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="0e3ba-116">· Dacă caracteristica este  *dezactivată*  , faceți clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="0e3ba-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="0e3ba-117">Pentru mai multe informații, vă rugăm să consultați următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="0e3ba-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

