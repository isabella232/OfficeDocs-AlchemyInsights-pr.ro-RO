---
title: Locația datelor
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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655294"
---
# <a name="data-location"></a>Locația datelor

Puteți vizualiza locația entității găzduite în centrul de administrare sau conectându-vă la Exchange Online prin PowerShell.


**Centru de administrare:**
1. Conectați-vă la centrul de [administrare](https://admin.microsoft.com/Adminportal/Home).
2. Selectaþi Profil**organizare** **setãri** > .
3. Sub **Locație date**, selectați Vizualizare **detalii**.


**Powershell:**
1. Conectați-vă la Exchange Online utilizând Windows PowerShell.
2. Executați cmdletul [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) pentru a afișa o listă a proprietăților entității găzduite. 
3. Uită-te la proprietatea OrganizationId.

Când aveți locația de date pentru EXO și SPO, puteți determina locația de date pentru alte servicii pe care le puteți utiliza din [Locul în care se află datele dvs.](https://products.office.com/where-is-your-data-located)