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
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="9c981-102">Canale private în Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9c981-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="9c981-103">Canalele private este o caracteristică nouă în Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9c981-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="9c981-104">Rețineți că canalele private nu pot fi convertite din canale standard sau invers.</span><span class="sxs-lookup"><span data-stu-id="9c981-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="9c981-105">Pentru detalii despre canalele private, ar fi informații despre [crearea canalelor private și calitatea de membru](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) și [site-urile SharePoint de canale private](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), consultați Canale private în Microsoft [Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="9c981-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="9c981-106">**Notã:** Deoarece configurarea pentru păstrarea mesajelor de canal privat nu este încă acceptată, entitățile găzduite cu politicile de conservare activate nu vor avea canale private activate în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="9c981-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="9c981-107">Canalele private pot fi activate în centrul de administrare Teams.</span><span class="sxs-lookup"><span data-stu-id="9c981-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="9c981-108">De asemenea, rețineți că, în timp ce păstrarea mesajelor de canal privat nu este acceptată, păstrarea fișierelor partajate în canale private este acceptată.</span><span class="sxs-lookup"><span data-stu-id="9c981-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="9c981-109">**Ai nevoie de un nou proprietar de echipă?**</span><span class="sxs-lookup"><span data-stu-id="9c981-109">**Need a new team owner?**</span></span>

<span data-ttu-id="9c981-110">Dacă proprietarul canalului privat pleacă, poți adăuga un nou proprietar de echipă prin Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="9c981-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="9c981-111">Du-te [aici](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) pentru a instala Echipe Powershell.</span><span class="sxs-lookup"><span data-stu-id="9c981-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="9c981-112">Aici este cmdlet-ul veți avea nevoie de:</span><span class="sxs-lookup"><span data-stu-id="9c981-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="9c981-113">Pentru mai multe informații despre Teams Powershell, consultați [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="9c981-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
