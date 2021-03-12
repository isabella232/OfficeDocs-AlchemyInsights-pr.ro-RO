---
title: Setările politicii de întâlnire
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704618"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="ca2af-102">Gestionarea politicilor de întâlnire în Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="ca2af-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="ca2af-103">**Notă: poate dura până la 24 de ore pentru ca modificările politice să aibă efect pentru utilizatori.**</span><span class="sxs-lookup"><span data-stu-id="ca2af-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="ca2af-104">Este posibil să nu reușiți să efectuați modificări imediat în politicile nou create; Așteptați 4 ore și încercați să modificați din nou o politică nou creată.</span><span class="sxs-lookup"><span data-stu-id="ca2af-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="ca2af-105">Politicile pentru întâlniri sunt utilizate pentru a controla caracteristicile disponibile pentru participanții la întâlnire pentru întâlnirile programate de utilizatorii din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="ca2af-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="ca2af-106">Este posibil ca unele caracteristici ale politicilor de întâlnire să nu fie implementate încă în centrul de administrare teams (acestea sunt etichetate "în curând" din documentație).</span><span class="sxs-lookup"><span data-stu-id="ca2af-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="ca2af-107">În acest caz, sau dacă primiți o eroare de genul "nu putem actualiza politica acum, dar încercați din nou mai târziu" în centrul de administrare Microsoft teams, vă recomandăm să utilizați PowerShell pentru a crea sau a modifica politicile întâlnirii teams.</span><span class="sxs-lookup"><span data-stu-id="ca2af-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="ca2af-108">Pentru mai multe informații despre politicile de întâlnire, consultați următoarele resurse:</span><span class="sxs-lookup"><span data-stu-id="ca2af-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="ca2af-109">Pentru a afla despre crearea politicilor, efectuarea de modificări și atribuirea de utilizatori la politică, consultați [gestionarea politicilor de întâlnire în teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="ca2af-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="ca2af-110">Pentru a face modificări de politică utilizând cmdleturi PowerShell, consultați [Prezentare generală teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="ca2af-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="ca2af-111">Trebuie să utilizați [modul Skype for Business PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) pentru politicile de întâlnire teams.</span><span class="sxs-lookup"><span data-stu-id="ca2af-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="ca2af-112">Revizuiți [documentația cmdleturilor \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="ca2af-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

