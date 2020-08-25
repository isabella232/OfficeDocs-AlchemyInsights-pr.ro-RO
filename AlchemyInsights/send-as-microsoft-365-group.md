---
title: Trimitere ca Microsoft 365 Group
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872090"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="9eafe-102">Trimitere ca Microsoft 365 Group</span><span class="sxs-lookup"><span data-stu-id="9eafe-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="9eafe-103">Puteți să atribuiți permisiuni trimitere ca pentru a permite anumitor utilizatori să trimită mesaje ca grup Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="9eafe-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="9eafe-104">Conectați-vă la Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9eafe-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="9eafe-105">Rulați următoarea comandă:</span><span class="sxs-lookup"><span data-stu-id="9eafe-105">Run the following command:</span></span>  

    <span data-ttu-id="9eafe-106">Add-RecipientPermission `<GroupName>` -mandatar `<MailboxName>` -AccessRights SendAs</span><span class="sxs-lookup"><span data-stu-id="9eafe-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="9eafe-107">Pentru mai multe informații, consultați [Permiteți membrilor să trimită sau să trimită în numele unui grup](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="9eafe-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>