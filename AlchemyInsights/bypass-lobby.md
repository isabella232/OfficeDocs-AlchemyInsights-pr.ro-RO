---
title: Bypass lobby
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684962"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="d059a-102">Controlați setările din lobby și nivelul de participare la teams</span><span class="sxs-lookup"><span data-stu-id="d059a-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="d059a-103">Dacă doriți să permiteți tuturor, inclusiv utilizatorilor prin dial-in, externe și anonimi, să **ocoliți lobby-ul**, utilizați PowerShell pentru a realiza această activitate.</span><span class="sxs-lookup"><span data-stu-id="d059a-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="d059a-104">Iată un exemplu de modificare a politicii globale a întâlnirii pentru organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="d059a-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="d059a-105">Acest cmdlet necesită în prezent utilizarea modulului Skype for Business PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d059a-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="d059a-106">Pentru a vă configura să utilizați acest cmdlet, consultați [gestionarea politicilor prin PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="d059a-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="d059a-107">După ce ați configurat o politică, trebuie să o aplicați utilizatorilor; sau, dacă ați modificat Politica globală, aceasta se va aplica automat pentru utilizatori.</span><span class="sxs-lookup"><span data-stu-id="d059a-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="d059a-108">Pentru orice modificare de politică, trebuie să așteptați cel puțin **4 ore până la 24 de ore** pentru ca politicile să aibă efect.</span><span class="sxs-lookup"><span data-stu-id="d059a-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="d059a-109">Asigurați-vă că revizuiți documentația de mai jos înainte de a face aceste modificări pentru a înțelege exact ce permite aceasta.</span><span class="sxs-lookup"><span data-stu-id="d059a-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="d059a-110">Înțelegerea controalelor politicii de lobby pentru întâlnirile teams</span><span class="sxs-lookup"><span data-stu-id="d059a-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="d059a-111">Aceste setări controlează ce participanții la întâlnire așteaptă în sala de așteptare înainte ca aceștia să fie admiși la întâlnire și nivelul de participare la care este permis într-o întâlnire.</span><span class="sxs-lookup"><span data-stu-id="d059a-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="d059a-112">Puteți utiliza PowerShell pentru a actualiza setările politicii de întâlnire care nu au fost implementate încă (etichetate "în curând") în centrul de administrare teams.</span><span class="sxs-lookup"><span data-stu-id="d059a-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="d059a-113">Vedeți mai jos pentru un exemplu de cmdlet PowerShell care permite tuturor utilizatorilor să ocolească lobby-ul.</span><span class="sxs-lookup"><span data-stu-id="d059a-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="d059a-114">[Admiteți automat că persoanele](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) sunt o politică per organizator care verifică dacă persoanele se asociază direct la o întâlnire sau așteaptă în lobby până când sunt admise de un utilizator autentificat.</span><span class="sxs-lookup"><span data-stu-id="d059a-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="d059a-115">[Permiteți persoanelor anonime să înceapă o întâlnire](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) este o politică per organizator care verifică dacă persoane anonime, inclusiv B2B și utilizatori federativi, pot participa la întâlnirea utilizatorului fără un utilizator autentificat din organizație în prezență.</span><span class="sxs-lookup"><span data-stu-id="d059a-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="d059a-116">[Permiteți utilizatorilor prin dial-in să ocolească sala de așteptare](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**în curând**) este o politică per-organizator care controlează dacă persoanele care apelează prin telefon se asociază direct la întâlnire sau așteaptă în lobby, indiferent de setarea de **persoane care admit automat** .</span><span class="sxs-lookup"><span data-stu-id="d059a-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="d059a-117">[Permiteți organizatorilor să ignore setările din lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**în curând**) este o politică per organizator care verifică dacă organizatorul întâlnirii poate să ignore setările din sala de așteptare pe care un administrator le-a setat în **mod automat să admită persoane** și **să permită utilizatorilor prin dial-in să ocolească lobby-** ul atunci când planifică o întâlnire nouă.</span><span class="sxs-lookup"><span data-stu-id="d059a-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="d059a-118">**Notă:** Citiți [gestionarea politicilor de întâlnire în teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) pentru o prezentare generală completă a politicilor de întâlnire Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="d059a-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
