---
title: Mesaj de întâmpinare în grupuri Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357836"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="20dfe-102">Mesaj de întâmpinare în grupuri Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="20dfe-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="20dfe-103">Utilizatorii noi care se alătură grupului Microsoft 365 vor primi un e-mail de bun venit dacă proprietatea "UnifiedGroupWelcomeMessageEnabled" este Adevărat.</span><span class="sxs-lookup"><span data-stu-id="20dfe-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="20dfe-104">În cazul în care doriți să dezactivați mesajul de întâmpinare, utilizați următoarea comandă [EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="20dfe-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
