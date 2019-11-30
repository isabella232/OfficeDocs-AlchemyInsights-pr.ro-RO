---
title: Locație de date
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627858"
---
# <a name="data-location"></a>Locație de date

Puteți vizualiza locația entității găzduite Office 365 în centrul de administrare sau prin conectarea la Exchange Online prin PowerShell.


**Centrul de administrare:**
1. Conectați-vă la [Centrul de administrare](https://admin.microsoft.com/Adminportal/Home).
2. Selectați **Setări** > **profil organizație**.
3. Sub **locație de date**, selectați **Vizualizați detaliile**.


**Powershell:**
1. Conectați-vă la Exchange Online utilizând Windows PowerShell.
2. Executați cmdletul [Get-Organizalunit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) pentru a afișa o listă de proprietățile entității găzduite. 
3. Uită-te la proprietatea OrganizationId.

Când aveți locația de date pentru EXO și SPO, puteți determina locația de date pentru alte servicii pe care le puteți utiliza de [unde se află datele](https://products.office.com/where-is-your-data-located).