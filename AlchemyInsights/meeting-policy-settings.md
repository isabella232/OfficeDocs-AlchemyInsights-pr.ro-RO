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
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704618"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gestionarea politicilor de întâlnire în Microsoft teams

**Notă: poate dura până la 24 de ore pentru ca modificările politice să aibă efect pentru utilizatori.** Este posibil să nu reușiți să efectuați modificări imediat în politicile nou create; Așteptați 4 ore și încercați să modificați din nou o politică nou creată.

Politicile pentru întâlniri sunt utilizate pentru a controla caracteristicile disponibile pentru participanții la întâlnire pentru întâlnirile programate de utilizatorii din organizația dvs. Este posibil ca unele caracteristici ale politicilor de întâlnire să nu fie implementate încă în centrul de administrare teams (acestea sunt etichetate "în curând" din documentație). În acest caz, sau dacă primiți o eroare de genul "nu putem actualiza politica acum, dar încercați din nou mai târziu" în centrul de administrare Microsoft teams, vă recomandăm să utilizați PowerShell pentru a crea sau a modifica politicile întâlnirii teams. 

Pentru mai multe informații despre politicile de întâlnire, consultați următoarele resurse:

- Pentru a afla despre crearea politicilor, efectuarea de modificări și atribuirea de utilizatori la politică, consultați [gestionarea politicilor de întâlnire în teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Pentru a face modificări de politică utilizând cmdleturi PowerShell, consultați [Prezentare generală teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Trebuie să utilizați [modul Skype for Business PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) pentru politicile de întâlnire teams. 
    - Revizuiți [documentația cmdleturilor *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) pentru mai multe informații.

