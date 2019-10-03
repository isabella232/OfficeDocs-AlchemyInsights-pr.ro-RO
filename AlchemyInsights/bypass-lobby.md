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
# <a name="control-lobby-settings-and-level-of-participation"></a>Setările lobby-ului de control și nivelul de participare

Aceste setări controlează care participanți la întâlnire așteaptă în lobby înainte de a fi admiși la întâlnire și nivelul de participare pe care sunt permise într-o întâlnire. Aveți posibilitatea să utilizați PowerShell pentru a actualiza setările de politică de întâlnire care nu au fost încă implementate (etichetate "în curând") în centrul de administrare echipe.  Consultați mai jos pentru un exemplu cmdlet PowerShell care permite tuturor utilizatorilor să ocolească lobby-ul.  

- [Recunoaște automat că persoanele](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) sunt o politică per organizator care controlează dacă persoanele se alătură direct unei întâlniri sau așteaptă în lobby până când sunt admise de un utilizator autentificat.

- [Permiteți persoanelor anonime să pornească o întâlnire](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) este o politică per-organizator care controlează dacă persoanele anonime, inclusiv utilizatorii B2B și Federați, se pot alătura întâlnirii utilizatorului fără un utilizator autentificat din organizație în prezență.

- [Permiteți utilizatorilor dial-in să ocolească lobby-ul](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (în**curând**) este o politică per organizator care controlează dacă persoanele care formează prin telefon se alătură direct întâlnirii sau așteaptă în lobby, indiferent de setarea **automată a admiterii persoanelor** .

- [Permiteți organizatorilor să suprascrie setările lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) -ului (**în curând**) este o politică per-organizator care controlează dacă organizatorul întâlnirii poate suprascrie setările de lobby pe care un administrator le-a setat în **mod automat să admită persoane** și să **permită dial-in utilizatorii să ocolească lobby-** ul când programează o nouă întâlnire.

**Notă:** Citiți [Gestionați politicile de întâlnire în echipe](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) pentru o prezentare generală completă a politicilor de întâlnire Microsoft teams. 


**Exemplu PowerShell**

Dacă doriți să permiteți tuturor, inclusiv utilizatorilor externi sau anonimi, să ocoliți lobby-ul, puteți utiliza și PowerShell pentru a realiza această activitate.  Iată un exemplu de modificare a politicii globale de întâlnire pentru organizația dvs.   

(Asigurați-vă că pentru a revizui documentația de mai sus înainte de a face aceste modificări pentru a înțelege exact ceea ce permite acest lucru.)

Set-CsTeamsMeetingPolicy-identitate global-AutoAdmittedUsers "toată lumea"-AllowPSTNUsersToBypassLobby $True

Pentru mai multe informații, consultați [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
