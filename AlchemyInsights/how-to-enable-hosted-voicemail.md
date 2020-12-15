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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679168"
---
# <a name="how-to-enable-hosted-voicemail"></a>Cum se activează mesageria vocală găzduită

Pentru a activa mesageria vocală, **HostedVoicemail** trebuie setată la $True.

Proprietatea **HostedVoicemail** a utilizatorului utilizând Remote POWERSHELL (RPS).

Pentru mai multe informații despre conectarea la RPS, consultați [prezentarea generală Microsoft teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) pentru mai multe informații despre conectarea la RPS.

1. Administratorul teams trebuie să fie conectat la Remote PowerShell pentru teams.
1. Din PowerShell prompt, administratorul teams poate executa **set-csuser user@contoso.com-HostedVoiceMail $True** în care SIP uri este al utilizatorului în cauză.

> [!NOTE]
> Modificările aduse politicilor pot dura până la 24 de ore pentru reproducere.