---
title: Recuperarea elementelor șterse cu cmdletul
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
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835823"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="92499-102">Recuperarea elementelor șterse cu cmdletul</span><span class="sxs-lookup"><span data-stu-id="92499-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="92499-103">Utilizați cmdletul [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) pentru a vizualiza elementele șterse din cutiile poștale.</span><span class="sxs-lookup"><span data-stu-id="92499-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="92499-104">După ce găsiți elementele șterse, utilizați cmdletul [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) pentru a le restaura.</span><span class="sxs-lookup"><span data-stu-id="92499-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="92499-105">Vedeți detaliile complete în [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="92499-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="92499-106">Trebuie să vă fie atribuit rolul de Import/Export pentru cutii poștale înainte de a putea rula acest cmdlet.</span><span class="sxs-lookup"><span data-stu-id="92499-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="92499-107">Consultați informațiile [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="92499-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
