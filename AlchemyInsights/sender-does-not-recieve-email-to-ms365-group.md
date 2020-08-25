---
title: Expeditorul nu primește mesaje de e-mail trimise la Microsoft 365 Group
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872088"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Expeditorul nu primește mesaje de e-mail trimise la Microsoft 365 Group

În mod implicit, expeditorul unui mesaj de e-mail către un grup Microsoft 365 nu primește o copie a mesajului în Inbox, chiar dacă expeditorul este membru al grupului.

Utilizați această comandă EXO PowerShell pentru a permite expeditorului să primească o copie a fiecărui mesaj de e-mail pe care îl trimit la grupul Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Pentru a activa setarea pentru toate cutiile poștale simultan:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Notă** Modificările aduse acestei setări durează până la o oră pentru a avea efect.