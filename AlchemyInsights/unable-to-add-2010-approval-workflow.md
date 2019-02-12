---
title: Imposibil de adăugat fluxul de lucru aprobare 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 3741b1169ddf731725c18fbaed80bfb321e5db46
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925428"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="859f8-102">Imposibil de adăugat fluxul de lucru aprobare 2010</span><span class="sxs-lookup"><span data-stu-id="859f8-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="859f8-103">Într-o colecţie de site-ul Microsoft SharePoint, nu puteţi adăuga un flux de lucru reutilizabil la nivel global (cum ar fi "aprobare - SharePoint 2010") o listă sau o bibliotecă.</span><span class="sxs-lookup"><span data-stu-id="859f8-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="859f8-104">Pentru a rezolva această problemă, urmaţi aceşti paşi:</span><span class="sxs-lookup"><span data-stu-id="859f8-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="859f8-105">Deschide site-ul rădăcină din colecția de site-ul în SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="859f8-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="859f8-106">Cu **Site-ul obiectele**, selectați **fluxuri de lucru**.</span><span class="sxs-lookup"><span data-stu-id="859f8-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="859f8-107">În secţiunea **noua** de panglica de **fluxuri de lucru** , selectaţi **Flux de lucru reutilizabil**.</span><span class="sxs-lookup"><span data-stu-id="859f8-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="859f8-p101">Formular **Creare flux de lucru reutilizabil** , introduceţi numele \*\* *Repair2010* \*\*. Pentru **Platforma de tip**, faceţi clic pe **Flux de lucru SharePoint 2010**, şi apoi faceţi clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="859f8-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="859f8-110">În secţiunea **Salvare** de panglica de **flux de lucru** , selectaţi **Publicare**.</span><span class="sxs-lookup"><span data-stu-id="859f8-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="859f8-p102">În secţiunea de **administrare** a panglicii de **flux de lucru** , selectaţi **Publica la nivel global**. În casetă de dialog de confirmare care apare, selectaţi **OK**.</span><span class="sxs-lookup"><span data-stu-id="859f8-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="859f8-p103">Într-un browser web, localizați site-ul rădăcină al colecției de site-uri, şi apoi accesa **Site-ul setările** \> **Caracteristici de colectare site-ului**. Comuta caracteristica de **fluxuri de lucru** :</span><span class="sxs-lookup"><span data-stu-id="859f8-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="859f8-115">· În cazul în care funcţia este *activ* , faceţi clic pe **Dezactivare,** şi apoi faceţi clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="859f8-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="859f8-116">· În cazul în care funcţia este *dezactivata* , faceţi clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="859f8-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="859f8-117">Pentru mai multe informaţii vă rugăm să consultaţi următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="859f8-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

