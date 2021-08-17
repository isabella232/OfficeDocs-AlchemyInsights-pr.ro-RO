---
title: Cum se activează mesageria vocală găzduită
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055566"
---
# <a name="how-to-enable-hosted-voicemail"></a>Cum se activează mesageria vocală găzduită

Pentru a activa mesageria **vocală, HostedVoicemail** trebuie să fie setată la $true.

Proprietatea **HostedVoicemail a** utilizatorului care utilizează PowerShell la distanță (RPS).

Pentru mai multe informații despre conectarea la RPS, [consultați prezentarea Microsoft Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) pentru mai multe informații despre conectarea la RPS.

1. Administratorul Teams ar trebui să fie conectat la PowerShell la distanță pentru Teams.
1. De la Solicitare PowerShell, administratorul Teams poate rula **set-csuser user@contoso.com -HostedVoiceMail $true** în care sip uri este al utilizatorului respectiv.

> [!NOTE]
> Reproducerea modificărilor politicilor poate dura până la 24 de ore.