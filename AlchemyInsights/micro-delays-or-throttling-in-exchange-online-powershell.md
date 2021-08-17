---
title: Microîntârzieri sau limitare în Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314712"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Microîntârzieri sau limitare în Exchange Online PowerShell

Este posibil să vedeți avertizările „Microîntârzieri aplicate” sau întârzieri atunci când rulați scripturi și cmdleturi în Exchange Online. Iată câteva sugestii despre cum să rezolvați acest lucru:

- Rulați diagnosticele noastre pentru a vă relaxa politicile de throtare PowerShell ale entității găzduite. Această soluție va rezolva problema în mare parte.
- Dacă problema tot nu se rezolvă, utilizați modulul [Exchange Online v2 PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)care include CMDleturi care se bazează pe REST API și sunt semnificativ mai performante. Aceasta poate fi o soluție foarte bună pentru multe dintre CMDleturile Obțineți- utilizate frecvent.
- Dacă trebuie să utilizați CMDleturi care nu sunt acoperite de modulul v2, consultați Rularea [cmdletelor PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)pentru un număr mare de utilizatori în Office 365 , care discută despre cum să ocoliți limitele de limitarea PowerShell în Exchange Online.
