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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830045"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Microîntârzieri sau limitare în Exchange Online PowerShell

Este posibil să vedeți avertizările „Microîntârzieri aplicate” sau întârzieri atunci când rulați scripturi și cmdleturi în Exchange Online. Iată două sugestii legate de aceasta:

- Poate că doriți să încercați să utilizați [modulul Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), care include CMDleturile bazate pe REST API și sunt cu mult mai performante. Aceasta poate fi o soluție foarte bună pentru multe dintre CMDleturile Obțineți- utilizate frecvent.
- Dacă trebuie să utilizați CMDleturi care nu sunt incluse încă în modulul v2, consultați [Rularea cmdleturilor PowerShell pentru un număr mare de utilizatori în Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), care arată cum să parcurgeți limitările PowerShell estimate din Exchange Online.
