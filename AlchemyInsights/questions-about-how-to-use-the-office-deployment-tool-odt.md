---
title: Întrebări despre cum să utilizaţi instrumentul de implementare Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925356"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Întrebări despre cum să utilizaţi instrumentul de implementare Office (ODT)

Descărcaţi instrumentul de implementare Office la [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
După descărcarea fişierului, executaţi fişierul executabil cu auto-extragere, care conţine birou implementare instrumentul executabil (setup.exe) şi un eşantion de fişier de configurare (einkommentiert).
  
 **Pentru a exclude sau de a elimina produsele Office 365 ProPlus din computerele client:**
  
Când instalaţi Office 365 ProPlus, puteţi exclude anumite produse. Pentru aceasta, urmați pașii pentru instalarea Office cu ODT, dar include elementul ExcludeApp în fişierul de configurare. De exemplu, acest fişier de configurare instalează toate produsele Office 365 ProPlus cu excepţia Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Prezentare generală a instrumentului de implementare Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

