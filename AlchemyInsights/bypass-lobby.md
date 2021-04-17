---
title: Ocolirea sala de așteptare
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820046"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="f5650-102">Controlul setărilor privind sala de așteptare și nivelul de participare în Teams</span><span class="sxs-lookup"><span data-stu-id="f5650-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="f5650-103">Dacă preferați să permiteți tuturor, inclusiv utilizatorilor externi, externi și anonimi, să ocolească sala de **așteptare,** utilizați PowerShell pentru a realiza această activitate.</span><span class="sxs-lookup"><span data-stu-id="f5650-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="f5650-104">Iată un exemplu de modificare a politicii globale pentru întâlniri pentru organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="f5650-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="f5650-105">Acest cmdlet necesită în prezent utilizarea modulului Skype for Business PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f5650-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="f5650-106">Pentru a configura utilizarea acestui cmdlet, consultați [Gestionarea politicilor prin PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="f5650-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="f5650-107">După ce ați configurat o politică, trebuie să o aplicați utilizatorilor; sau, dacă modificați politica globală, aceasta se va aplica automat utilizatorilor.</span><span class="sxs-lookup"><span data-stu-id="f5650-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="f5650-108">Pentru orice modificare de politică, trebuie să așteptați cel puțin 4 ore până **la 24 de** ore pentru ca politicile să aibă efect.</span><span class="sxs-lookup"><span data-stu-id="f5650-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="f5650-109">Nu trebuie să consultați documentația de mai jos înainte de a face aceste modificări pentru a înțelege exact ce permite acest lucru.</span><span class="sxs-lookup"><span data-stu-id="f5650-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="f5650-110">Înțelegerea controalelor politicii privind sala de așteptare pentru întâlnirile Teams</span><span class="sxs-lookup"><span data-stu-id="f5650-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="f5650-111">Aceste setări controlează ce participanți la întâlnire așteaptă în sala de așteptare înainte de a fi admiși la întâlnire și nivelul de participare la întâlnire.</span><span class="sxs-lookup"><span data-stu-id="f5650-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="f5650-112">Puteți utiliza PowerShell pentru a actualiza setările politicii pentru întâlniri care nu au fost implementate încă (etichetate cu "în curând") în centrul de administrare Teams.</span><span class="sxs-lookup"><span data-stu-id="f5650-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="f5650-113">Vedeți mai jos un exemplu de cmdlet PowerShell care le permite tuturor utilizatorilor să ocolească sala de așteptare.</span><span class="sxs-lookup"><span data-stu-id="f5650-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="f5650-114">[Admiterea automată a persoanelor](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) este o politică pentru fiecare organizator care controlează dacă persoanele se alătură unei întâlniri direct sau așteaptă în sala de așteptare până când sunt admise de un utilizator autentificat.</span><span class="sxs-lookup"><span data-stu-id="f5650-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="f5650-115">[](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Permiteți persoanelor anonime să inițieze o întâlnire este o politică pentru fiecare organizator care controlează dacă persoanele anonime, inclusiv utilizatorii B2B și utilizatorii federativi, se pot alătura la întâlnirea utilizatorului fără să fie prezent un utilizator autentificat din organizație.</span><span class="sxs-lookup"><span data-stu-id="f5650-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="f5650-116">Permiteți utilizatorilor prin [dial-in](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) să ocolească sala de așteptare **(în** curând) este o politică pentru fiecare organizator  care controlează dacă persoanele care apelează prin telefon se alătură întâlnirii direct sau așteaptă în sala de așteptare, indiferent de setarea Admite automat persoane.</span><span class="sxs-lookup"><span data-stu-id="f5650-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="f5650-117">[Permite organizatorilor](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) să suprascrie setările sălii de așteptare **(în** curând) este o politică a organizatorului  care controlează dacă organizatorul întâlnirii poate înlocui setările sălii de așteptare configurate de administrator în Permiteți utilizatorilor prin **dial-in** să ocolească sala de așteptare atunci când programează o nouă întâlnire.</span><span class="sxs-lookup"><span data-stu-id="f5650-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="f5650-118">**Notă:** Citiți [Gestionarea politicilor pentru întâlniri în Teams pentru](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) o prezentare generală completă a politicilor pentru întâlnirile Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f5650-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
