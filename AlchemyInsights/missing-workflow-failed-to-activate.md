---
title: Lipsă de flux de lucru nu a reuşit pentru a activa
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 33b92c2cae1f641b0cd88c82fd4ae5e8632d76c2
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28307662"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="cca2c-102">Lipsă de flux de lucru nu a reuşit pentru a activa</span><span class="sxs-lookup"><span data-stu-id="cca2c-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="cca2c-103">Într-o colecţie de site-ul Microsoft SharePoint, nu puteţi adăuga un flux de lucru reutilizabil la nivel global (cum ar fi "aprobare - SharePoint 2010") o listă sau o bibliotecă.</span><span class="sxs-lookup"><span data-stu-id="cca2c-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="cca2c-104">Pentru a rezolva această problemă, urmaţi aceşti paşi:</span><span class="sxs-lookup"><span data-stu-id="cca2c-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="cca2c-105">Deschide site-ul rădăcină din colecția de site-ul în SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="cca2c-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="cca2c-106">Cu **Site-ul obiectele**, selectați **fluxuri de lucru**.</span><span class="sxs-lookup"><span data-stu-id="cca2c-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="cca2c-107">În secţiunea **noua** de panglica de **fluxuri de lucru** , selectaţi **Flux de lucru reutilizabil**.</span><span class="sxs-lookup"><span data-stu-id="cca2c-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="cca2c-p101">Formular **Creare flux de lucru reutilizabil** , introduceţi numele \*\* *Repair2010* \*\*. Pentru **Platforma de tip**, faceţi clic pe **Flux de lucru SharePoint 2010**, şi apoi faceţi clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="cca2c-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="cca2c-110">În secţiunea **Salvare** de panglica de **flux de lucru** , selectaţi **Publicare**.</span><span class="sxs-lookup"><span data-stu-id="cca2c-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="cca2c-p102">În secţiunea de **administrare** a panglicii de **flux de lucru** , selectaţi **Publica la nivel global**. În casetă de dialog de confirmare care apare, selectaţi **OK**.</span><span class="sxs-lookup"><span data-stu-id="cca2c-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="cca2c-p103">Într-un browser web, localizați site-ul rădăcină al colecției de site-uri, şi apoi accesa **Site-ul setările** \> **Caracteristici de colectare site-ului**. Apoi, comuta caracteristica de **fluxuri de lucru** :</span><span class="sxs-lookup"><span data-stu-id="cca2c-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="cca2c-115">· În cazul în care funcţia este *activ* , faceţi clic pe **Dezactivare,** şi apoi faceţi clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="cca2c-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="cca2c-116">· În cazul în care funcţia este *dezactivata* , faceţi clic pe **Activare**.</span><span class="sxs-lookup"><span data-stu-id="cca2c-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="cca2c-117">Pentru mai multe informaţii vă rugăm să consultaţi următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="cca2c-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

