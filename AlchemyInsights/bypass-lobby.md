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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Controlați setările din lobby și nivelul de participare la teams

Dacă doriți să permiteți tuturor, inclusiv utilizatorilor prin dial-in, externe și anonimi, să **ocoliți lobby-ul**, utilizați PowerShell pentru a realiza această activitate. Iată un exemplu de modificare a politicii globale a întâlnirii pentru organizația dvs.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Acest cmdlet necesită în prezent utilizarea modulului Skype for Business PowerShell. Pentru a vă configura să utilizați acest cmdlet, consultați [gestionarea politicilor prin PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

După ce ați configurat o politică, trebuie să o aplicați utilizatorilor; sau, dacă ați modificat Politica globală, aceasta se va aplica automat pentru utilizatori. Pentru orice modificare de politică, trebuie să așteptați cel puțin **4 ore până la 24 de ore** pentru ca politicile să aibă efect. 

Asigurați-vă că revizuiți documentația de mai jos înainte de a face aceste modificări pentru a înțelege exact ce permite aceasta.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Înțelegerea controalelor politicii de lobby pentru întâlnirile teams

Aceste setări controlează ce participanții la întâlnire așteaptă în sala de așteptare înainte ca aceștia să fie admiși la întâlnire și nivelul de participare la care este permis într-o întâlnire. Puteți utiliza PowerShell pentru a actualiza setările politicii de întâlnire care nu au fost implementate încă (etichetate "în curând") în centrul de administrare teams. Vedeți mai jos pentru un exemplu de cmdlet PowerShell care permite tuturor utilizatorilor să ocolească lobby-ul.

- [Admiteți automat că persoanele](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) sunt o politică per organizator care verifică dacă persoanele se asociază direct la o întâlnire sau așteaptă în lobby până când sunt admise de un utilizator autentificat.

- [Permiteți persoanelor anonime să înceapă o întâlnire](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) este o politică per organizator care verifică dacă persoane anonime, inclusiv B2B și utilizatori federativi, pot participa la întâlnirea utilizatorului fără un utilizator autentificat din organizație în prezență.

- [Permiteți utilizatorilor prin dial-in să ocolească sala de așteptare](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**în curând**) este o politică per-organizator care controlează dacă persoanele care apelează prin telefon se asociază direct la întâlnire sau așteaptă în lobby, indiferent de setarea de **persoane care admit automat** .

- [Permiteți organizatorilor să ignore setările din lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**în curând**) este o politică per organizator care verifică dacă organizatorul întâlnirii poate să ignore setările din sala de așteptare pe care un administrator le-a setat în **mod automat să admită persoane** și **să permită utilizatorilor prin dial-in să ocolească lobby-** ul atunci când planifică o întâlnire nouă.

**Notă:** Citiți [gestionarea politicilor de întâlnire în teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) pentru o prezentare generală completă a politicilor de întâlnire Microsoft teams.
