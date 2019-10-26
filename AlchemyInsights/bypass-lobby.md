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
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/25/2019
ms.locfileid: "37654268"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Setările lobby-ului de control și nivelul de participare

Dacă doriți să permiteți tuturor, inclusiv utilizatorilor dial-in, externi și anonimi să ocolească lobby-ul, puteți utiliza PowerShell pentru a o face. Iată un exemplu de modificare a politicii globale de întâlnire pentru organizația dvs.:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Acest cmdlet necesită în prezent utilizarea Skype pentru afaceri PowerShell modulul. Pentru a obține instalarea pentru a utiliza acest cmdlet, consultați [gestionarea politicilor prin intermediul PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Aveți posibilitatea să configurați o politică nouă, pe care va trebui apoi să o aplicați utilizatorilor. Dacă modificați politica globală, aceasta se va aplica automat utilizatorilor. Pentru orice schimbare de politică trebuie să așteptați cel puțin 4 ore și până la 24 de ore pentru ca politicile să aibă efect.

Asigurați-vă că pentru a revizui documentația de mai jos înainte de a face aceste modificări pentru a înțelege exact ceea ce permite acest lucru.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Înțelegerea echipelor de întâlnire controale politica lobby

- [Recunoaște automat că persoanele](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) sunt o politică per organizator care controlează dacă persoanele se alătură direct unei întâlniri sau așteaptă în lobby până când sunt admise de un utilizator autentificat.

- [Permiteți persoanelor anonime să pornească o întâlnire](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) este o politică per-organizator care controlează dacă persoanele anonime, inclusiv utilizatorii B2B și Federați, se pot alătura întâlnirii utilizatorului fără un utilizator autentificat din organizație în prezență.

- [Permiteți utilizatorilor dial-in să ocolească lobby-ul](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (în**curând**) este o politică per organizator care controlează dacă persoanele care formează prin telefon se alătură direct întâlnirii sau așteaptă în lobby, indiferent de setarea **automată a admiterii persoanelor** .

- [Permiteți organizatorilor să suprascrie setările lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) -ului (**în curând**) este o politică per-organizator care controlează dacă organizatorul întâlnirii poate suprascrie setările de lobby pe care un administrator le-a setat în **mod automat să admită persoane** și să **permită dial-in utilizatorii să ocolească lobby-** ul când programează o nouă întâlnire.

**Notă:** Citiți [Gestionați politicile de întâlnire în echipe](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) pentru o prezentare generală completă a politicilor de întâlnire Microsoft teams.
