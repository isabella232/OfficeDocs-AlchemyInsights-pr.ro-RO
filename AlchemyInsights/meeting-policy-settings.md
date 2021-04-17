---
title: Setările politicii pentru întâlniri
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825455"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="1fe13-102">Gestionarea politicilor pentru întâlniri în Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="1fe13-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="1fe13-103">**Notă: poate dura până la 24 de ore pentru ca modificările politicii să aibă efect pentru utilizatori.**</span><span class="sxs-lookup"><span data-stu-id="1fe13-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="1fe13-104">Este posibil să nu puteți efectua imediat modificări la politicile nou create; așteptați 4 ore și încercați să modificați din nou o politică nou creată.</span><span class="sxs-lookup"><span data-stu-id="1fe13-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="1fe13-105">Politicile de întâlnire sunt utilizate pentru a controla caracteristicile disponibile participanților la întâlnire pentru întâlnirile programate de utilizatorii din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="1fe13-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="1fe13-106">Este posibil ca unele caracteristici ale politicilor pentru întâlniri să nu fie implementate încă în centrul de administrare Teams (acestea sunt etichetate cu "în curând" în documentație).</span><span class="sxs-lookup"><span data-stu-id="1fe13-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="1fe13-107">În acest caz sau dacă primiți o eroare precum "Nu putem actualiza politica în acest moment, dar încercați din nou mai târziu" din Centrul de administrare Microsoft Teams, vă recomandăm să utilizați PowerShell pentru a crea sau a modifica politicile întâlnirilor Teams.</span><span class="sxs-lookup"><span data-stu-id="1fe13-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="1fe13-108">Pentru mai multe informații despre politicile de întâlnire, consultați următoarele resurse:</span><span class="sxs-lookup"><span data-stu-id="1fe13-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="1fe13-109">Pentru a afla despre crearea politicilor, efectuarea de modificări și atribuirea utilizatorilor în politică, consultați Gestionarea politicilor [pentru întâlniri în Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="1fe13-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="1fe13-110">Pentru a face modificări de politică utilizând cmdleturi PowerShell, consultați [Prezentare generală Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="1fe13-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="1fe13-111">Trebuie să utilizați modulul [Skype for Business PowerShell pentru politicile](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) întâlnirii Teams.</span><span class="sxs-lookup"><span data-stu-id="1fe13-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="1fe13-112">Consultați [documentația cmdleturilor \*-CsTeamsMeetingPolicy pentru mai](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) multe informații.</span><span class="sxs-lookup"><span data-stu-id="1fe13-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

