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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376789"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="732dc-102">Setările lobby-ului de control și nivelul de participare</span><span class="sxs-lookup"><span data-stu-id="732dc-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="732dc-103">Aceste setări controlează care participanți la întâlnire așteaptă în lobby înainte de a fi admiși la întâlnire și nivelul de participare pe care sunt permise într-o întâlnire.</span><span class="sxs-lookup"><span data-stu-id="732dc-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="732dc-104">Aveți posibilitatea să utilizați PowerShell pentru a actualiza setările de politică de întâlnire care nu au fost încă implementate (etichetate "în curând") în centrul de administrare echipe.</span><span class="sxs-lookup"><span data-stu-id="732dc-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="732dc-105">Consultați mai jos pentru un exemplu cmdlet PowerShell care permite tuturor utilizatorilor să ocolească lobby-ul.</span><span class="sxs-lookup"><span data-stu-id="732dc-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="732dc-106">[Recunoaște automat că persoanele](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) sunt o politică per organizator care controlează dacă persoanele se alătură direct unei întâlniri sau așteaptă în lobby până când sunt admise de un utilizator autentificat.</span><span class="sxs-lookup"><span data-stu-id="732dc-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="732dc-107">[Permiteți persoanelor anonime să pornească o întâlnire](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) este o politică per-organizator care controlează dacă persoanele anonime, inclusiv utilizatorii B2B și Federați, se pot alătura întâlnirii utilizatorului fără un utilizator autentificat din organizație în prezență.</span><span class="sxs-lookup"><span data-stu-id="732dc-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="732dc-108">[Permiteți utilizatorilor dial-in să ocolească lobby-ul](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (în**curând**) este o politică per organizator care controlează dacă persoanele care formează prin telefon se alătură direct întâlnirii sau așteaptă în lobby, indiferent de setarea **automată a admiterii persoanelor** .</span><span class="sxs-lookup"><span data-stu-id="732dc-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="732dc-109">[Permiteți organizatorilor să suprascrie setările lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) -ului (**în curând**) este o politică per-organizator care controlează dacă organizatorul întâlnirii poate suprascrie setările de lobby pe care un administrator le-a setat în **mod automat să admită persoane** și să **permită dial-in utilizatorii să ocolească lobby-** ul când programează o nouă întâlnire.</span><span class="sxs-lookup"><span data-stu-id="732dc-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="732dc-110">**Notă:** Citiți [Gestionați politicile de întâlnire în echipe](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) pentru o prezentare generală completă a politicilor de întâlnire Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="732dc-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="732dc-111">**Exemplu PowerShell**</span><span class="sxs-lookup"><span data-stu-id="732dc-111">**PowerShell example**</span></span>

<span data-ttu-id="732dc-112">Dacă doriți să permiteți tuturor, inclusiv utilizatorilor externi sau anonimi, să ocoliți lobby-ul, puteți utiliza și PowerShell pentru a realiza această activitate.</span><span class="sxs-lookup"><span data-stu-id="732dc-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="732dc-113">Iată un exemplu de modificare a politicii globale de întâlnire pentru organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="732dc-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="732dc-114">(Asigurați-vă că pentru a revizui documentația de mai sus înainte de a face aceste modificări pentru a înțelege exact ceea ce permite acest lucru.)</span><span class="sxs-lookup"><span data-stu-id="732dc-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="732dc-115">Set-CsTeamsMeetingPolicy-identitate global-AutoAdmittedUsers "toată lumea"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="732dc-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="732dc-116">Pentru mai multe informații, consultați [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="732dc-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
