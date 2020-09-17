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
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774903"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Întrebări despre cum să utilizați instrumentul de implementare Office (ODT)

Descărcați instrumentul de implementare Office de la [Centrul de descărcare Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
După ce descărcați fișierul, rulați fișierul executabil cu auto-extragere, care conține executabilul instrumentului de implementare Office (setup.exe) și un fișier de configurare eșantion (configuration.xml).
  
 **Pentru a exclude sau a elimina aplicațiile Microsoft 365 pentru produsele Enterprise de pe computerele client:**
  
Atunci când instalați aplicații Microsoft 365 pentru întreprinderi, puteți să excludeți anumite produse. Pentru a face acest lucru, urmați pașii pentru instalarea Office cu ODT, dar includeți elementul ExcludeApp în fișierul de configurare. De exemplu, acest fișier de configurare instalează toate aplicațiile Microsoft 365 pentru produsele Enterprise, cu excepția Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Prezentare generală a instrumentului de implementare Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

