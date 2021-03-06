---
title: Mesajele trimise către grupul Microsoft 365 nu sunt primite de toți membrii
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: d222eb92d806bad52264139a8ddba72f323b3783
ms.sourcegitcommit: 10cfd9d552b0d8a096bcef34e82c04a4c166a13a
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50479465"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Mesajele trimise către un grup Microsoft 365 nu sunt primite de toți membrii

Asigurați-vă că toți membrii grupului s-au abonat să primească mesajele de e-mail. Consultați [Urmărirea unui grup în Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Pentru a verifica starea mesajului pentru membrii care s-au abonat la mesaje de e-mail de grup, rulați următoarea comandă în [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Utilizați următoarea comandă EXO PowerShell pentru a configura toți membrii grupului să primească în inbox mesajele de e-mail trimise către grupul Microsoft 365:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

De exemplu:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`