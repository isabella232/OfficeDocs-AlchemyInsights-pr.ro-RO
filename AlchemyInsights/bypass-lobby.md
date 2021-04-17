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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Controlul setărilor privind sala de așteptare și nivelul de participare în Teams

Dacă preferați să permiteți tuturor, inclusiv utilizatorilor externi, externi și anonimi, să ocolească sala de **așteptare,** utilizați PowerShell pentru a realiza această activitate. Iată un exemplu de modificare a politicii globale pentru întâlniri pentru organizația dvs.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Acest cmdlet necesită în prezent utilizarea modulului Skype for Business PowerShell. Pentru a configura utilizarea acestui cmdlet, consultați [Gestionarea politicilor prin PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

După ce ați configurat o politică, trebuie să o aplicați utilizatorilor; sau, dacă modificați politica globală, aceasta se va aplica automat utilizatorilor. Pentru orice modificare de politică, trebuie să așteptați cel puțin 4 ore până **la 24 de** ore pentru ca politicile să aibă efect. 

Nu trebuie să consultați documentația de mai jos înainte de a face aceste modificări pentru a înțelege exact ce permite acest lucru.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Înțelegerea controalelor politicii privind sala de așteptare pentru întâlnirile Teams

Aceste setări controlează ce participanți la întâlnire așteaptă în sala de așteptare înainte de a fi admiși la întâlnire și nivelul de participare la întâlnire. Puteți utiliza PowerShell pentru a actualiza setările politicii pentru întâlniri care nu au fost implementate încă (etichetate cu "în curând") în centrul de administrare Teams. Vedeți mai jos un exemplu de cmdlet PowerShell care le permite tuturor utilizatorilor să ocolească sala de așteptare.

- [Admiterea automată a persoanelor](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) este o politică pentru fiecare organizator care controlează dacă persoanele se alătură unei întâlniri direct sau așteaptă în sala de așteptare până când sunt admise de un utilizator autentificat.

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Permiteți persoanelor anonime să inițieze o întâlnire este o politică pentru fiecare organizator care controlează dacă persoanele anonime, inclusiv utilizatorii B2B și utilizatorii federativi, se pot alătura la întâlnirea utilizatorului fără să fie prezent un utilizator autentificat din organizație.

- Permiteți utilizatorilor prin [dial-in](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) să ocolească sala de așteptare **(în** curând) este o politică pentru fiecare organizator  care controlează dacă persoanele care apelează prin telefon se alătură întâlnirii direct sau așteaptă în sala de așteptare, indiferent de setarea Admite automat persoane.

- [Permite organizatorilor](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) să suprascrie setările sălii de așteptare **(în** curând) este o politică a organizatorului  care controlează dacă organizatorul întâlnirii poate înlocui setările sălii de așteptare configurate de administrator în Permiteți utilizatorilor prin **dial-in** să ocolească sala de așteptare atunci când programează o nouă întâlnire.

**Notă:** Citiți [Gestionarea politicilor pentru întâlniri în Teams pentru](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) o prezentare generală completă a politicilor pentru întâlnirile Microsoft Teams.
