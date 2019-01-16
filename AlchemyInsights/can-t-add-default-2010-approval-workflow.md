---
title: Imposibil de adăugat implicit fluxul de lucru aprobare 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28306558"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="d0578-102">Imposibil de adăugat implicit fluxul de lucru aprobare 2010</span><span class="sxs-lookup"><span data-stu-id="d0578-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="d0578-103">Într-o colecţie de site-ul Microsoft SharePoint, nu puteţi adăuga un flux de lucru reutilizabil la nivel global (cum ar fi "aprobare - SharePoint 2010") o listă sau o bibliotecă.</span><span class="sxs-lookup"><span data-stu-id="d0578-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="d0578-104">Pentru a rezolva această problemă, urmaţi aceşti paşi:</span><span class="sxs-lookup"><span data-stu-id="d0578-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="d0578-105">Deschide site-ul rădăcină din colecția de site-ul în SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="d0578-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="d0578-106">Cu **Site-ul obiectele**, selectați **fluxuri de lucru**.</span><span class="sxs-lookup"><span data-stu-id="d0578-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="d0578-107">În secţiunea **noua** de panglica de **fluxuri de lucru** , selectaţi **Flux de lucru reutilizabil**.</span><span class="sxs-lookup"><span data-stu-id="d0578-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="d0578-p101">Formular **Creare flux de lucru reutilizabil** , introduceţi numele \* \*\*Repair2010\*\*\*. Pentru **Platforma de tip**, selectaţi **Flux de lucru SharePoint 2010**, şi apoi selectaţi **OK**.</span><span class="sxs-lookup"><span data-stu-id="d0578-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="d0578-110">În secţiunea **Salvare** de panglica de **flux de lucru** , selectaţi **Publicare**.</span><span class="sxs-lookup"><span data-stu-id="d0578-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="d0578-p102">În secţiunea de **administrare** a panglicii de **flux de lucru** , selectaţi **Publica la nivel global**. În casetă de dialog de confirmare care apare, selectaţi **OK**.</span><span class="sxs-lookup"><span data-stu-id="d0578-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="d0578-p103">Într-un browser web, localizați site-ul rădăcină al colecției de site-uri, şi apoi accesa **Site-ul setările** \> **Caracteristici de colectare site-ului**. Apoi, comuta caracteristica de **fluxuri de lucru** :</span><span class="sxs-lookup"><span data-stu-id="d0578-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="d0578-115">· În cazul în care funcţia este *activ* , faceţi clic pe **Dezactivare,** şi apoi faceţi clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="d0578-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="d0578-116">· În cazul în care funcţia este *dezactivata* , faceţi clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="d0578-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="d0578-117">Pentru mai multe informaţii vă rugăm să consultaţi următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="d0578-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

