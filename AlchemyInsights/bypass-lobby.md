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
ms.openlocfilehash: 5ee77e57b3bc64d7a04256ab67b691e5205eac56
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/27/2019
ms.locfileid: "39626360"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="0ad4f-102">Setările lobby-ului de control și nivelul de participare</span><span class="sxs-lookup"><span data-stu-id="0ad4f-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="0ad4f-103">Dacă doriți să permiteți tuturor, inclusiv utilizatorilor dial-in, externi și anonimi să ocolească lobby-ul în Microsoft teams, puteți utiliza PowerShell pentru a o face.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="0ad4f-104">Iată un exemplu de modificare a politicii globale de întâlnire pentru organizația dvs.:</span><span class="sxs-lookup"><span data-stu-id="0ad4f-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="0ad4f-105">Acest cmdlet necesită în prezent utilizarea Skype pentru afaceri PowerShell modulul.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="0ad4f-106">Pentru a obține instalarea pentru a utiliza acest cmdlet, consultați [gestionarea politicilor prin intermediul PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="0ad4f-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="0ad4f-107">Aveți posibilitatea să configurați o politică nouă, pe care va trebui apoi să o aplicați utilizatorilor.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="0ad4f-108">Dacă modificați politica globală, aceasta se va aplica automat utilizatorilor.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="0ad4f-109">Pentru orice schimbare de politică trebuie să așteptați cel puțin 4 ore și până la 24 de ore pentru ca politicile să aibă efect.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="0ad4f-110">Asigurați-vă că pentru a revizui documentația de mai jos înainte de a face aceste modificări pentru a înțelege exact ceea ce permite acest lucru.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="0ad4f-111">Înțelegerea echipelor de întâlnire controale politica lobby</span><span class="sxs-lookup"><span data-stu-id="0ad4f-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="0ad4f-112">[Recunoaște automat că persoanele](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) sunt o politică per organizator care controlează dacă persoanele se alătură direct unei întâlniri sau așteaptă în lobby până când sunt admise de un utilizator autentificat.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="0ad4f-113">[Permiteți persoanelor anonime să pornească o întâlnire](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) este o politică per-organizator care controlează dacă persoanele anonime, inclusiv utilizatorii B2B și Federați, se pot alătura întâlnirii utilizatorului fără un utilizator autentificat din organizație în prezență.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="0ad4f-114">[Permiteți utilizatorilor dial-in să ocolească lobby-ul](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (în**curând**) este o politică per organizator care controlează dacă persoanele care formează prin telefon se alătură direct întâlnirii sau așteaptă în lobby, indiferent de setarea **automată a admiterii persoanelor** .</span><span class="sxs-lookup"><span data-stu-id="0ad4f-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="0ad4f-115">[Permiteți organizatorilor să suprascrie setările lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) -ului (**în curând**) este o politică per-organizator care controlează dacă organizatorul întâlnirii poate suprascrie setările de lobby pe care un administrator le-a setat în **mod automat să admită persoane** și **să permită utilizatorilor dial-in să ocolească lobby-** ul când programează o nouă întâlnire.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="0ad4f-116">**Notă:** Citiți [Gestionați politicile de întâlnire în echipe](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) pentru o prezentare generală completă a politicilor de întâlnire Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="0ad4f-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
