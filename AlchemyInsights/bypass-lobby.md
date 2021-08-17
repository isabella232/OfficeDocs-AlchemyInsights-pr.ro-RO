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
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059608"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Controlul setărilor privind sala de așteptare și nivelul de participare Teams

Dacă preferați să permiteți tuturor, inclusiv utilizatorilor externi, externi și anonimi, să ocolească sala de **așteptare,** utilizați PowerShell pentru a realiza această activitate. Iată un exemplu de modificare a politicii globale pentru întâlniri pentru organizația dvs.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Acest cmdlet necesită în prezent utilizarea Skype for Business PowerShell. Pentru a configura utilizarea acestui cmdlet, consultați [Gestionarea politicilor prin PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

După ce ați configurat o politică, trebuie să o aplicați utilizatorilor; sau, dacă modificați politica globală, aceasta se va aplica automat utilizatorilor. Pentru orice modificare de politică, trebuie să așteptați cel puțin 4 ore până **la 24 de** ore pentru ca politicile să aibă efect. 

Nu trebuie să consultați documentația de mai jos înainte de a face aceste modificări pentru a înțelege exact ce permite acest lucru.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Înțelegerea Teams politicii privind sala de așteptare a întâlnirii

Aceste setări controlează ce participanți la întâlnire așteaptă în sala de așteptare înainte de a fi admiși la întâlnire și nivelul de participare la întâlnire. Puteți utiliza PowerShell pentru a actualiza setările politicii pentru întâlniri care nu au fost implementate încă (etichetate cu "în curând") în centrul Teams administrare. Vedeți mai jos un exemplu de cmdlet PowerShell care le permite tuturor utilizatorilor să ocolească sala de așteptare.

- [Admiterea automată a persoanelor](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) este o politică pentru fiecare organizator care controlează dacă persoanele se alătură unei întâlniri direct sau așteaptă în sala de așteptare până când sunt admise de un utilizator autentificat.

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Permiteți persoanelor anonime să inițieze o întâlnire este o politică pentru fiecare organizator care controlează dacă persoanele anonime, inclusiv utilizatorii B2B și utilizatorii federativi, se pot alătura la întâlnirea utilizatorului fără să fie prezent un utilizator autentificat din organizație.

- Permiteți utilizatorilor prin [dial-in](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) să ocolească sala de așteptare **(în** curând) este o politică pentru fiecare organizator  care controlează dacă persoanele care apelează prin telefon se alătură întâlnirii direct sau așteaptă în sala de așteptare, indiferent de setarea Admite automat persoane.

- [Permite organizatorilor](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) să suprascrie setările sălii de așteptare **(în** curând) este o politică a organizatorului  care controlează dacă organizatorul întâlnirii poate înlocui setările sălii de așteptare configurate de administrator în Permiteți utilizatorilor prin **dial-in** să ocolească sala de așteptare atunci când programează o nouă întâlnire.

**Notă:** Citiți [Gestionarea politicilor pentru întâlniri în Teams pentru](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) o prezentare generală completă a Microsoft Teams privind întâlnirile.
