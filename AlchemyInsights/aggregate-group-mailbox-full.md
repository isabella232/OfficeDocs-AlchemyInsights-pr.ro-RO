---
title: AggregateGroupMailbox full NDR received for email sent to Microsoft 365 group
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315922"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox full NDR received for email sent to Microsoft 365 group

Utilizați următoarea comandă EXO Shell pentru a crea o regulă de transport Exchange și a fixa în mod silențios mesajele de e-mail trimise la cutia poștală de grup agregată:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Notă:** Înlocuiți adresa SMTP din **-SentTo cu adresa** SMTP a cutiei poștale de grup agregate din entitatea dvs. găzduită. Puteți obține adresa SMTP a cutiei poștale de grup agregate din NDR primit.



