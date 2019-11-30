---
title: Setările politicii de întâlnire
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627586"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="040e9-102">Gestionați politicile de întâlnire în Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="040e9-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="040e9-103">Politicile de întâlnire sunt utilizate pentru a controla caracteristicile care sunt disponibile pentru a întâlni participanți pentru întâlniri care sunt programate de către utilizatorii din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="040e9-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="040e9-104">Este posibil ca unele caracteristici ale politicilor de întâlnire să nu fie implementate în centrul de administrare a echipelor încă (acestea sunt etichetate "în curând" în documentație).</span><span class="sxs-lookup"><span data-stu-id="040e9-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="040e9-105">În acest caz, sau dacă se obține o eroare de genul "nu putem actualiza politica chiar acum, dar încercați din nou mai târziu" în centrul de administrare Microsoft teams, vă recomandăm să utilizați PowerShell pentru a crea sau modifica echipele de întâlnire politici.</span><span class="sxs-lookup"><span data-stu-id="040e9-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="040e9-106">Pentru mai multe informații despre politicile de întâlnire, consultați următoarele resurse:</span><span class="sxs-lookup"><span data-stu-id="040e9-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="040e9-107">Pentru a afla despre crearea politicilor, efectuarea modificărilor și asocierea utilizatorilor la politică, consultați [gestionarea politicilor de întâlnire în echipe](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="040e9-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="040e9-108">Pentru a face modificări de politică utilizând cmdleturi PowerShell, consultați [Prezentare generală a echipelor PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="040e9-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="040e9-109">Trebuie să utilizați [Skype pentru afaceri PowerShell modulul](https://www.microsoft.com/download/details.aspx?id=39366) pentru echipele de întâlnire politici.</span><span class="sxs-lookup"><span data-stu-id="040e9-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="040e9-110">Examinați [documentația \*-csteamsmeetingpolicy cmdlet](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="040e9-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="040e9-111">**Notă:** Poate dura până la 24 de ore pentru ca modificările de politică să aibă efect pentru utilizatori.</span><span class="sxs-lookup"><span data-stu-id="040e9-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="040e9-112">Este posibil să nu puteți modifica imediat politicile nou create; Așteptați 4 ore și încercați să modificați din nou o politică nou creată.</span><span class="sxs-lookup"><span data-stu-id="040e9-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="040e9-113">Dacă încă întâmpinați probleme, încercați PowerShell.</span><span class="sxs-lookup"><span data-stu-id="040e9-113">If you're still having problems, try PowerShell.</span></span>  