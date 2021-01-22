---
title: Activarea tehnologiei,
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935136"
---
# <a name="turn-on-ndi-technology"></a>Activarea tehnologiei,

Tehnologia, pentru un utilizator, trebuie să fie activate doi pași:

1. Administratorul entității găzduite trebuie să activeze proprietatea ' AllowNDIStreaming ' în CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. După ce această modificare a fost populată, utilizatorul final trebuie să activeze tehnologia®, pentru clientul său specific, din **permisiunile > permisiuni**.

Pentru mai multe informații, consultați [utilizarea tehnologiei, în Microsoft teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
