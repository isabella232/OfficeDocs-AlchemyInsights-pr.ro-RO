---
title: Mesajele trimise către grupul Microsoft 365 nu sunt primite de toți membrii
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.contentlocale: ro-RO
ms.lasthandoff: 07/06/2020
ms.locfileid: "45051514"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="074ea-102">Mesajele trimise către un grup Microsoft 365 nu sunt primite de toți membrii</span><span class="sxs-lookup"><span data-stu-id="074ea-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="074ea-103">Asigurați-vă că toți membrii grupului s-au abonat pentru a primi e-mailurile.</span><span class="sxs-lookup"><span data-stu-id="074ea-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="074ea-104">Consultați [Urmărirea unui grup în Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="074ea-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="074ea-105">Pentru a verifica starea mesajului membrilor care s-au abonat la e-mailurile de grup, executați următoarea comandă pe [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="074ea-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`