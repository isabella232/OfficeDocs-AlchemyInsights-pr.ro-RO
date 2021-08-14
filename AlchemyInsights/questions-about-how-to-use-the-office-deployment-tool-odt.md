---
title: Întrebări despre utilizarea instrumentului de Office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959695"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Întrebări despre utilizarea instrumentului de Office (ODT)

Descărcați instrumentul Office de implementare locală din [Centrul de descărcare Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
După descărcarea fișierului, rulați fișierul executabil auto extras, care conține instrumentul de implementare Office executabil (setup.exe) și un exemplu de fișier de configurare (configuration.xml).
  
 **Pentru a exclude sau a Aplicații Microsoft 365 pentru întreprindere produse de pe computerele client:**
  
Atunci când instalați Aplicații Microsoft 365 pentru întreprindere, puteți exclude anumite produse. Pentru a face acest lucru, urmați pașii pentru Office ODT, dar includeți elementul ExcludeApp în fișierul de configurare. De exemplu, acest fișier de configurare instalează toate produsele Aplicații Microsoft 365 pentru întreprindere, cu excepția Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Prezentare generală a Instrumentului Office implementare](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

