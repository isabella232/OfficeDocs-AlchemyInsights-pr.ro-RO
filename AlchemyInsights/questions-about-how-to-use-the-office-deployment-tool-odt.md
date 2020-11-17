---
title: Întrebări despre cum să utilizați instrumentul de implementare Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086168"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="29fe6-102">Întrebări despre cum să utilizați instrumentul de implementare Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="29fe6-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="29fe6-103">Descărcați instrumentul de implementare Office de la [Centrul de descărcare Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="29fe6-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="29fe6-104">După ce descărcați fișierul, rulați fișierul executabil cu auto-extragere, care conține executabilul instrumentului de implementare Office (setupodt.exe) și un fișier de configurare eșantion (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="29fe6-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="29fe6-105">**Pentru a exclude sau a elimina aplicațiile Microsoft 365 pentru produsele Enterprise de pe computerele client:**</span><span class="sxs-lookup"><span data-stu-id="29fe6-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="29fe6-106">Atunci când instalați aplicații Microsoft 365 pentru întreprinderi, puteți să excludeți anumite produse.</span><span class="sxs-lookup"><span data-stu-id="29fe6-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="29fe6-107">Pentru a face acest lucru, urmați pașii pentru instalarea Office cu ODT, dar includeți elementul ExcludeApp în fișierul de configurare.</span><span class="sxs-lookup"><span data-stu-id="29fe6-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="29fe6-108">De exemplu, acest fișier de configurare instalează toate aplicațiile Microsoft 365 pentru produsele Enterprise, cu excepția Publisher:</span><span class="sxs-lookup"><span data-stu-id="29fe6-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="29fe6-109">Prezentare generală a instrumentului de implementare Office</span><span class="sxs-lookup"><span data-stu-id="29fe6-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

