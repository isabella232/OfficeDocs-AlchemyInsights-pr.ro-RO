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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="be6ec-102">Microîntârzieri sau limitare în Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="be6ec-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="be6ec-103">Este posibil să vedeți avertizările „Microîntârzieri aplicate” sau întârzieri atunci când rulați scripturi și cmdleturi în Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="be6ec-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="be6ec-104">Iată două sugestii legate de aceasta:</span><span class="sxs-lookup"><span data-stu-id="be6ec-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="be6ec-105">Poate că doriți să încercați să utilizați [modulul Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), care include CMDleturile bazate pe REST API și sunt cu mult mai performante.</span><span class="sxs-lookup"><span data-stu-id="be6ec-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="be6ec-106">Aceasta poate fi o soluție foarte bună pentru multe dintre CMDleturile Obțineți- utilizate frecvent.</span><span class="sxs-lookup"><span data-stu-id="be6ec-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="be6ec-107">Dacă trebuie să utilizați CMDleturi care nu sunt incluse încă în modulul v2, consultați [Rularea cmdleturilor PowerShell pentru un număr mare de utilizatori în Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), care arată cum să parcurgeți limitările PowerShell estimate din Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="be6ec-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
