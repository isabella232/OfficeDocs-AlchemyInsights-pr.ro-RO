---
title: Utilizarea Giphy în conversațiile teams
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
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982580"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="68035-102">Utilizarea Giphy în conversațiile teams</span><span class="sxs-lookup"><span data-stu-id="68035-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="68035-103">Accesul giphy în teams chat este activat în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="68035-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="68035-104">Ca administrator, puteți să controlați dacă Giphy sunt disponibili pentru utilizatori [setând o politică de mesagerie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) și asigurându-vă că **Utilizați giphy în conversații** este **activată**.</span><span class="sxs-lookup"><span data-stu-id="68035-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="68035-105">Dacă GIF-urile nu funcționează așa cum vă așteptați în conversațiile teams, verificați:</span><span class="sxs-lookup"><span data-stu-id="68035-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="68035-106">[Politica de mesagerie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) trebuie să permită giphy.</span><span class="sxs-lookup"><span data-stu-id="68035-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="68035-107">Pentru a verifica dacă utilizați cmdleturi PowerShell:</span><span class="sxs-lookup"><span data-stu-id="68035-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="68035-108">Verificați dacă puteți [gestiona teams cu PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="68035-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="68035-109">Executarea comenzii PowerShell [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) și verificați dacă **AllowGiphy** este setată la **True**.</span><span class="sxs-lookup"><span data-stu-id="68035-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="68035-110">Dacă **AllowGiphy** este setată la **false** , rulează următorul set de comenzi PowerShell [-CsTeamsMessagingPolicy-identity global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="68035-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="68035-111">[Experiențele conectate opționale](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) trebuie activate pentru a permite accesul la adresa URL Giphy.</span><span class="sxs-lookup"><span data-stu-id="68035-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="68035-112">Dacă aveți mai multe politici de mesagerie pentru echipe configurate pentru entitatea găzduită, puteți determina identitatea politicii atribuite utilizatorului afectat cu comanda PowerShell [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Selectați TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="68035-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
