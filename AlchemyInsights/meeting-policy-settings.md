---
title: Setările politicii de întâlnire
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794346"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gestionarea politicilor de întâlnire în Microsoft teams

**Notă: poate dura până la 24 de ore pentru ca modificările politice să aibă efect pentru utilizatori.** Este posibil să nu reușiți să efectuați modificări imediat în politicile nou create; Așteptați 4 ore și încercați să modificați din nou o politică nou creată.

Politicile pentru întâlniri sunt utilizate pentru a controla caracteristicile disponibile pentru participanții la întâlnire pentru întâlnirile programate de utilizatorii din organizația dvs. Este posibil ca unele caracteristici ale politicilor de întâlnire să nu fie implementate încă în centrul de administrare teams (acestea sunt etichetate "în curând" din documentație). În acest caz, sau dacă primiți o eroare de genul "nu putem actualiza politica acum, dar încercați din nou mai târziu" în centrul de administrare Microsoft teams, vă recomandăm să utilizați PowerShell pentru a crea sau a modifica politicile întâlnirii teams. 

Pentru mai multe informații despre politicile de întâlnire, consultați următoarele resurse:

- Pentru a afla despre crearea politicilor, efectuarea de modificări și atribuirea de utilizatori la politică, consultați [gestionarea politicilor de întâlnire în teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Pentru a face modificări de politică utilizând cmdleturi PowerShell, consultați [Prezentare generală teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Trebuie să utilizați [modul Skype for Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) pentru politicile de întâlnire teams. 
    - Revizuiți [documentația cmdleturilor *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) pentru mai multe informații.

