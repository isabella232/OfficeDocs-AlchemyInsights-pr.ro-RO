---
title: Microîntârzieri sau limitare în Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947902"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Microîntârzieri sau limitare în Exchange Online PowerShell

Este posibil să vedeți avertizările „Microîntârzieri aplicate” sau întârzieri atunci când rulați scripturi și cmdleturi în Exchange Online. Iată două sugestii legate de aceasta:

- Poate că doriți să încercați să utilizați [modulul Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), care include CMDleturile bazate pe REST API și sunt cu mult mai performante. Aceasta poate fi o soluție foarte bună pentru multe dintre CMDleturile Obțineți- utilizate frecvent.
- Dacă trebuie să utilizați CMDleturi care nu sunt incluse încă în modulul v2, consultați [Rularea cmdleturilor PowerShell pentru un număr mare de utilizatori în Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), care arată cum să parcurgeți limitările PowerShell estimate din Exchange Online.
