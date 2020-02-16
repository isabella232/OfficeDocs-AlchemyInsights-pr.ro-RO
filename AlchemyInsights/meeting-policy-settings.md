---
title: Setări de politică de întâlnire
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042856"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="6743d-102">Gestionarea politicilor de întâlnire în Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6743d-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="6743d-103">**Notă: poate dura până la 24 de ore pentru ca modificările de politică să aibă efect pentru utilizatori.**</span><span class="sxs-lookup"><span data-stu-id="6743d-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="6743d-104">Este posibil să nu puteți modifica imediat politicile nou create; așteptați 4 ore și încercați să modificați din nou o politică nou creată.</span><span class="sxs-lookup"><span data-stu-id="6743d-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="6743d-105">Politicile de întâlnire sunt utilizate pentru a controla caracteristicile disponibile participanților la întâlnire pentru întâlnirile programate de utilizatorii din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="6743d-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="6743d-106">Este posibil ca unele caracteristici ale politicilor de întâlnire să nu fie implementate încă în centrul de administrare Teams (acestea sunt etichetate "în curând" în documentație).</span><span class="sxs-lookup"><span data-stu-id="6743d-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="6743d-107">În acest caz, sau dacă primiți o eroare de genul "Nu putem actualiza politica chiar acum, dar încercați-l din nou mai târziu" în Centrul de administrare Microsoft Teams, vă recomandăm să utilizați PowerShell pentru a crea sau modifica politicile de întâlnire Echipe.</span><span class="sxs-lookup"><span data-stu-id="6743d-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="6743d-108">Pentru mai multe informații despre politicile de întâlnire, consultați următoarele resurse:</span><span class="sxs-lookup"><span data-stu-id="6743d-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="6743d-109">Pentru a afla despre crearea politicilor, efectuarea de modificări și atribuirea utilizatorilor la politică, consultați [Gestionarea politicilor](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)de întâlnire în Echipe .</span><span class="sxs-lookup"><span data-stu-id="6743d-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="6743d-110">Pentru a efectua modificări de politică utilizând cmdlet-uri PowerShell, consultați [Prezentare generală PowerShell pentru echipe](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="6743d-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="6743d-111">Trebuie să utilizați [skype pentru afaceri PowerShell modul pentru](https://www.microsoft.com/download/details.aspx?id=39366) echipe politicile de întâlnire.</span><span class="sxs-lookup"><span data-stu-id="6743d-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="6743d-112">Examinați [documentația cmdlet-urilor \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="6743d-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

