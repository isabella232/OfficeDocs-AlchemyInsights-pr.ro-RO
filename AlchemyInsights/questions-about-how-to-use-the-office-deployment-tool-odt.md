---
title: Întrebări despre se utilizează Instrumentul de implementare Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698070"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="a9576-102">Întrebări despre se utilizează Instrumentul de implementare Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="a9576-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="a9576-103">Descărcați instrumentul de implementare Office din Centrul de [descărcare Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="a9576-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="a9576-104">După descărcarea fișierului, executați fișierul executabil de auto-extragere, care conține executabilul Instrument de implementare Office (setup.exe) și un fișier de configurare eșantion (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="a9576-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="a9576-105">**Pentru a exclude sau elimina Microsoft 365 Apps for enterprise produse de pe computerele client:**</span><span class="sxs-lookup"><span data-stu-id="a9576-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="a9576-106">Atunci când instalați Microsoft 365 Apps pentru întreprinderi, puteți exclude anumite produse.</span><span class="sxs-lookup"><span data-stu-id="a9576-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="a9576-107">Pentru a face acest lucru, urmați pașii pentru instalarea Office cu ODT, dar includeți elementul ExcludeApp în fișierul de configurare.</span><span class="sxs-lookup"><span data-stu-id="a9576-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="a9576-108">De exemplu, acest fișier de configurare instalează toate microsoft 365 Apps for enterprise produse, cu excepția Publisher:</span><span class="sxs-lookup"><span data-stu-id="a9576-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="a9576-109">Prezentare generală a instrumentului de implementare Office</span><span class="sxs-lookup"><span data-stu-id="a9576-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

