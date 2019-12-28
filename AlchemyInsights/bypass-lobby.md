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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Controlează setările lobby-ului și nivelul de participare la echipe

Dacă doriți să permiteți tuturor, inclusiv utilizatorilor dial-in, externi și anonimi, să **ocoliți lobby-ul**, utilizați PowerShell pentru a realiza această activitate. Iată un exemplu de modificare a politicii globale de întâlnire pentru organizația dvs.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Acest cmdlet necesită în prezent utilizarea Skype pentru afaceri PowerShell modulul. Pentru a obține configurat pentru a utiliza acest cmdlet, a verifica afară [gestionarea politicilor prin intermediul PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

După ce configurați o politică, trebuie să o aplicați utilizatorilor; sau, dacă ați modificat Politica globală, aceasta se va aplica automat utilizatorilor. Pentru orice schimbare de politică, trebuie să așteptați cel puțin **4 ore până la 24 de ore** pentru ca politicile să aibă efect. 

Asigurați-vă că pentru a revizui documentația de mai jos înainte de a face aceste modificări pentru a înțelege exact ceea ce permite acest lucru.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Înțelegerea echipelor de întâlnire controale politica lobby

Aceste setări controlează care participanți la întâlnire așteaptă în lobby înainte de a fi admiși la întâlnire și nivelul de participare pe care sunt permise într-o întâlnire. Aveți posibilitatea să utilizați PowerShell pentru a actualiza setările de politică de întâlnire care nu au fost încă implementate (etichetate "în curând") în centrul de administrare echipe. Consultați mai jos pentru un exemplu cmdlet PowerShell care permite tuturor utilizatorilor să ocolească lobby-ul.

- [Recunoaște automat că persoanele](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) sunt o politică per organizator care controlează dacă persoanele se alătură direct unei întâlniri sau așteaptă în lobby până când sunt admise de un utilizator autentificat.

- [Permiteți persoanelor anonime să pornească o întâlnire](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) este o politică per-organizator care controlează dacă persoanele anonime, inclusiv utilizatorii B2B și Federați, se pot alătura întâlnirii utilizatorului fără un utilizator autentificat din organizație în prezență.

- [Permiteți utilizatorilor dial-in să ocolească lobby-ul](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (în**curând**) este o politică per organizator care controlează dacă persoanele care formează prin telefon se alătură direct întâlnirii sau așteaptă în lobby, indiferent de setarea **automată a admiterii persoanelor** .

- [Permiteți organizatorilor să suprascrie setările lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) -ului (**în curând**) este o politică per-organizator care controlează dacă organizatorul întâlnirii poate suprascrie setările de lobby pe care un administrator le-a setat în **mod automat să admită persoane** și **să permită utilizatorilor dial-in să ocolească lobby-** ul când programează o nouă întâlnire.

**Notă:** Citiți [Gestionați politicile de întâlnire în echipe](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) pentru o prezentare generală completă a politicilor de întâlnire Microsoft teams.
