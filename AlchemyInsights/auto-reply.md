---
title: 'Pentru a configura răspunsul automat pentru toate mesajele de e-mail Microsoft 365 grup:'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: 3ed937d38627c1089c9203550498ce7b21ce01c0c5a2deea7326f8057f5338d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036144"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>Pentru a configura răspunsul automat pentru toate mesajele de e-mail Microsoft 365 grup:

**Conectare EXO PowerShell utilizând contul de administrator al entității găzduite și utilizați următoarea comandă:**

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> Schimbați **caseta de mesaj a** grupului cu un nume de grup pentru care doriți să configurați răspunsul automat.

