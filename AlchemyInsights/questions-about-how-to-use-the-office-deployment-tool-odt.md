---
title: Întrebări despre se utilizează instrumentul de implementare Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553552"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="625c6-102">Întrebări despre se utilizează instrumentul de implementare Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="625c6-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="625c6-103">Descărcați instrumentul de implementare Office de la [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="625c6-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="625c6-104">După descărcarea fișierului, executați fișierul executabil cu auto-extragere, care conține instrumentul de implementare Office executabil (Setup. exe) și un fișier de configurare eșantion (Configuration. xml).</span><span class="sxs-lookup"><span data-stu-id="625c6-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="625c6-105">**Pentru a exclude sau elimina Office 365 ProPlus produse de la computerele client:**</span><span class="sxs-lookup"><span data-stu-id="625c6-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="625c6-106">La instalarea Office 365 ProPlus, aveți posibilitatea să excludeți anumite produse.</span><span class="sxs-lookup"><span data-stu-id="625c6-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="625c6-107">Pentru aceasta, urmați pașii pentru instalarea Office cu ODT, dar includeți elementul ExcludeApp în fișierul de configurare.</span><span class="sxs-lookup"><span data-stu-id="625c6-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="625c6-108">De exemplu, acest fișier de configurare instalează toate produsele Office 365 ProPlus cu excepția Publisher:</span><span class="sxs-lookup"><span data-stu-id="625c6-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="625c6-109">Prezentare generală a instrumentului de implementare Office</span><span class="sxs-lookup"><span data-stu-id="625c6-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

