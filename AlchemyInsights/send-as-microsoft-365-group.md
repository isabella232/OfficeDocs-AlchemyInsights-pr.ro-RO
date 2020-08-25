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
# <a name="send-as-microsoft-365-group"></a>Trimitere ca Microsoft 365 Group

Puteți să atribuiți permisiuni trimitere ca pentru a permite anumitor utilizatori să trimită mesaje ca grup Microsoft 365:  

1. Conectați-vă la Exchange Online PowerShell.  

2. Rulați următoarea comandă:  

    Add-RecipientPermission `<GroupName>` -mandatar `<MailboxName>` -AccessRights SendAs

Pentru mai multe informații, consultați [Permiteți membrilor să trimită sau să trimită în numele unui grup](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).