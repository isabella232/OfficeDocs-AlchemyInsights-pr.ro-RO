---
title: Activarea tehnologiei NDI
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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023534"
---
# <a name="turn-on-ndi-technology"></a>Activarea tehnologiei NDI

Tehnologia NDI necesită două etape pentru a fi activată pentru un utilizator:

1. Administratorul entității găzduite trebuie să activeze proprietatea "AllowNDIStreaming" în CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. După ce această modificare s-a completat, utilizatorul final trebuie să activați tehnologia NDI® pentru clientul său specific **din Setări > permisiuni**.

Pentru mai multe informații, [consultați Utilizarea tehnologiei NDI în Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
