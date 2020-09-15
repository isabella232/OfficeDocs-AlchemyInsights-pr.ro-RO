---
title: Fluxul de lucru lipsă nu a putut fi activat
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667098"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="69c62-102">Fluxul de lucru lipsă nu a putut fi activat</span><span class="sxs-lookup"><span data-stu-id="69c62-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="69c62-103">Într-o colecție de site-uri Microsoft SharePoint, nu puteți adăuga un flux de lucru reutilizabil global (cum ar fi "aprobare-SharePoint 2010") într-o listă sau o bibliotecă.</span><span class="sxs-lookup"><span data-stu-id="69c62-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="69c62-104">Pentru a rezolva această problemă, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="69c62-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="69c62-105">Deschideți site-ul web rădăcină al colecției de site-uri în SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="69c62-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="69c62-106">Sub **obiecte site**, selectați **fluxuri de lucru**.</span><span class="sxs-lookup"><span data-stu-id="69c62-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="69c62-107">În secțiunea **nouă** a panglicii **fluxuri de lucru** , selectați **flux de lucru reutilizabil**.</span><span class="sxs-lookup"><span data-stu-id="69c62-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="69c62-108">În formularul **Creați un flux de lucru reutilizabil** , introduceți numele \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="69c62-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="69c62-109">Pentru **tip platformă**, faceți clic pe **flux de lucru SharePoint 2010**, apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="69c62-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="69c62-110">În secțiunea **Salvare** a panglicii **fluxului de lucru** , selectați **Publicare**.</span><span class="sxs-lookup"><span data-stu-id="69c62-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="69c62-111">În secțiunea **gestionare** a panglicii **fluxului de lucru** , selectați **Publicare la nivel global**.</span><span class="sxs-lookup"><span data-stu-id="69c62-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="69c62-112">În caseta de dialog de confirmare care apare, selectați **OK**.</span><span class="sxs-lookup"><span data-stu-id="69c62-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="69c62-113">Într-un browser web, găsiți site-ul web rădăcină al colecției de site **Site Settings** -uri, apoi accesați \> **caracteristicile colecției**site-ului setări site.</span><span class="sxs-lookup"><span data-stu-id="69c62-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="69c62-114">Apoi, comutați caracteristica **fluxuri de lucru** :</span><span class="sxs-lookup"><span data-stu-id="69c62-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="69c62-115">· Dacă caracteristica este  *activată*  , faceți clic pe Dezactivare **,** apoi faceți clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="69c62-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="69c62-116">· Dacă caracteristica este  *dezactivată*  , faceți clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="69c62-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="69c62-117">Pentru mai multe informații, vă rugăm să consultați următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="69c62-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

