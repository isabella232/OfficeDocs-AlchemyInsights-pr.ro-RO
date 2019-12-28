---
title: Bypass lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889094"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="32eb9-102">Controlează setările lobby-ului și nivelul de participare la echipe</span><span class="sxs-lookup"><span data-stu-id="32eb9-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="32eb9-103">Dacă doriți să permiteți tuturor, inclusiv utilizatorilor dial-in, externi și anonimi, să **ocoliți lobby-ul**, utilizați PowerShell pentru a realiza această activitate.</span><span class="sxs-lookup"><span data-stu-id="32eb9-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="32eb9-104">Iată un exemplu de modificare a politicii globale de întâlnire pentru organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="32eb9-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="32eb9-105">Acest cmdlet necesită în prezent utilizarea Skype pentru afaceri PowerShell modulul.</span><span class="sxs-lookup"><span data-stu-id="32eb9-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="32eb9-106">Pentru a obține configurat pentru a utiliza acest cmdlet, a verifica afară [gestionarea politicilor prin intermediul PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="32eb9-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="32eb9-107">După ce configurați o politică, trebuie să o aplicați utilizatorilor; sau, dacă ați modificat Politica globală, aceasta se va aplica automat utilizatorilor.</span><span class="sxs-lookup"><span data-stu-id="32eb9-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="32eb9-108">Pentru orice schimbare de politică, trebuie să așteptați cel puțin **4 ore până la 24 de ore** pentru ca politicile să aibă efect.</span><span class="sxs-lookup"><span data-stu-id="32eb9-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="32eb9-109">Asigurați-vă că pentru a revizui documentația de mai jos înainte de a face aceste modificări pentru a înțelege exact ceea ce permite acest lucru.</span><span class="sxs-lookup"><span data-stu-id="32eb9-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="32eb9-110">Înțelegerea echipelor de întâlnire controale politica lobby</span><span class="sxs-lookup"><span data-stu-id="32eb9-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="32eb9-111">Aceste setări controlează care participanți la întâlnire așteaptă în lobby înainte de a fi admiși la întâlnire și nivelul de participare pe care sunt permise într-o întâlnire.</span><span class="sxs-lookup"><span data-stu-id="32eb9-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="32eb9-112">Aveți posibilitatea să utilizați PowerShell pentru a actualiza setările de politică de întâlnire care nu au fost încă implementate (etichetate "în curând") în centrul de administrare echipe.</span><span class="sxs-lookup"><span data-stu-id="32eb9-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="32eb9-113">Consultați mai jos pentru un exemplu cmdlet PowerShell care permite tuturor utilizatorilor să ocolească lobby-ul.</span><span class="sxs-lookup"><span data-stu-id="32eb9-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="32eb9-114">[Recunoaște automat că persoanele](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) sunt o politică per organizator care controlează dacă persoanele se alătură direct unei întâlniri sau așteaptă în lobby până când sunt admise de un utilizator autentificat.</span><span class="sxs-lookup"><span data-stu-id="32eb9-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="32eb9-115">[Permiteți persoanelor anonime să pornească o întâlnire](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) este o politică per-organizator care controlează dacă persoanele anonime, inclusiv utilizatorii B2B și Federați, se pot alătura întâlnirii utilizatorului fără un utilizator autentificat din organizație în prezență.</span><span class="sxs-lookup"><span data-stu-id="32eb9-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="32eb9-116">[Permiteți utilizatorilor dial-in să ocolească lobby-ul](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (în**curând**) este o politică per organizator care controlează dacă persoanele care formează prin telefon se alătură direct întâlnirii sau așteaptă în lobby, indiferent de setarea **automată a admiterii persoanelor** .</span><span class="sxs-lookup"><span data-stu-id="32eb9-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="32eb9-117">[Permiteți organizatorilor să suprascrie setările lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) -ului (**în curând**) este o politică per-organizator care controlează dacă organizatorul întâlnirii poate suprascrie setările de lobby pe care un administrator le-a setat în **mod automat să admită persoane** și **să permită utilizatorilor dial-in să ocolească lobby-** ul când programează o nouă întâlnire.</span><span class="sxs-lookup"><span data-stu-id="32eb9-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="32eb9-118">**Notă:** Citiți [Gestionați politicile de întâlnire în echipe](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) pentru o prezentare generală completă a politicilor de întâlnire Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="32eb9-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
