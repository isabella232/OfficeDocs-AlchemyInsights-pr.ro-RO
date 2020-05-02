---
title: Canal privat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005450"
---
# <a name="private-channels-in-microsoft-teams"></a>Canale private în Microsoft Teams

Canalele private este o caracteristică nouă în Microsoft Teams. Rețineți că canalele private nu pot fi convertite din canale standard sau invers.

Pentru detalii despre canalele private, ar fi informații despre [crearea canalelor private și calitatea de membru](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) și [site-urile SharePoint de canale private](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), consultați Canale private în Microsoft [Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Notã:** Deoarece configurarea pentru păstrarea mesajelor de canal privat nu este încă acceptată, entitățile găzduite cu politicile de conservare activate nu vor avea canale private activate în mod implicit. Canalele private pot fi activate în centrul de administrare Teams. De asemenea, rețineți că, în timp ce păstrarea mesajelor de canal privat nu este acceptată, păstrarea fișierelor partajate în canale private este acceptată.

**Ai nevoie de un nou proprietar de echipă?**

Dacă proprietarul canalului privat pleacă, poți adăuga un nou proprietar de echipă prin Teams Powershell.


- Du-te [aici](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) pentru a instala Echipe Powershell.

Aici este cmdlet-ul veți avea nevoie de:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Pentru mai multe informații despre Teams Powershell, consultați [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
