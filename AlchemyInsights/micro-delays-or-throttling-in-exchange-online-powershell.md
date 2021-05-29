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
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702138"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="7f46d-102">Microîntârzieri sau limitare în Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="7f46d-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="7f46d-103">Este posibil să vedeți avertizările „Microîntârzieri aplicate” sau întârzieri atunci când rulați scripturi și cmdleturi în Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="7f46d-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="7f46d-104">Iată câteva sugestii despre cum să rezolvați această problemă:</span><span class="sxs-lookup"><span data-stu-id="7f46d-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="7f46d-105">Rulați diagnosticele noastre pentru a vă relaxa politicile de throtare PowerShell ale entității găzduite.</span><span class="sxs-lookup"><span data-stu-id="7f46d-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="7f46d-106">Această soluție va rezolva problema în mare parte.</span><span class="sxs-lookup"><span data-stu-id="7f46d-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="7f46d-107">Dacă problema tot nu se rezolvă, utilizați modulul [Exchange Online v2 PowerShell,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)care include CMDleturi care se bazează pe REST API și sunt semnificativ mai performante.</span><span class="sxs-lookup"><span data-stu-id="7f46d-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="7f46d-108">Aceasta poate fi o soluție foarte bună pentru multe dintre CMDleturile Obțineți- utilizate frecvent.</span><span class="sxs-lookup"><span data-stu-id="7f46d-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="7f46d-109">Dacă trebuie să utilizați CMDleturi care nu sunt acoperite în modulul v2, consultați Rularea [cmdletelor PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)pentru un număr mare de utilizatori în Office 365 , care discută despre cum să ocoliți limitele de limitarea PowerShell în Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="7f46d-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
