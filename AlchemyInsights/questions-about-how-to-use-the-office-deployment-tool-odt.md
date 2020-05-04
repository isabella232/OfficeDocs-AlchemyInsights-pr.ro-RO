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
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010765"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Întrebări despre se utilizează Instrumentul de implementare Office (ODT)

Descărcați instrumentul de implementare Office din Centrul de [descărcare Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
După descărcarea fișierului, executați fișierul executabil de auto-extragere, care conține executabilul Instrument de implementare Office (setup.exe) și un fișier de configurare eșantion (configuration.xml).
  
 **Pentru a exclude sau elimina Microsoft 365 Apps for enterprise produse de pe computerele client:**
  
Atunci când instalați Microsoft 365 Apps pentru întreprinderi, puteți exclude anumite produse. Pentru a face acest lucru, urmați pașii pentru instalarea Office cu ODT, dar includeți elementul ExcludeApp în fișierul de configurare. De exemplu, acest fișier de configurare instalează toate microsoft 365 Apps for enterprise produse, cu excepția Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Prezentare generală a instrumentului de implementare Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

