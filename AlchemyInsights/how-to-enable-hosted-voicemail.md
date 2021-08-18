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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318660"
---
# <a name="how-to-enable-hosted-voicemail"></a>Cum se activează mesageria vocală găzduită

Pentru a activa mesageria **vocală, HostedVoicemail** trebuie să fie setată la $true.

Proprietatea **HostedVoicemail a** utilizatorului care utilizează PowerShell la distanță (RPS).

Pentru mai multe informații despre conectarea la RPS, [consultați Prezentarea generală Microsoft Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) pentru mai multe informații despre conectarea la RPS.

1. Administratorul de Teams ar trebui să fie conectat la PowerShell la distanță pentru Teams.
1. Din Solicitare PowerShell, administratorul Teams poate rula **set-csuser user@contoso.com -HostedVoiceMail $true** în care sip uri este al utilizatorului respectiv.

**Notă:** modificarea politicilor poate dura până la 24 de ore pentru a fi reproduse.