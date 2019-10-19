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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Întrebări despre se utilizează instrumentul de implementare Office (ODT)

Descărcați instrumentul de implementare Office de la [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
După descărcarea fișierului, executați fișierul executabil cu auto-extragere, care conține instrumentul de implementare Office executabil (Setup. exe) și un fișier de configurare eșantion (Configuration. xml).
  
 **Pentru a exclude sau elimina Office 365 ProPlus produse de la computerele client:**
  
La instalarea Office 365 ProPlus, aveți posibilitatea să excludeți anumite produse. Pentru aceasta, urmați pașii pentru instalarea Office cu ODT, dar includeți elementul ExcludeApp în fișierul de configurare. De exemplu, acest fișier de configurare instalează toate produsele Office 365 ProPlus cu excepția Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Prezentare generală a instrumentului de implementare Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

