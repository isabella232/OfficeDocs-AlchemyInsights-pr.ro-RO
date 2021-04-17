---
title: Setările politicii pentru întâlniri
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825455"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gestionarea politicilor pentru întâlniri în Microsoft Teams

**Notă: poate dura până la 24 de ore pentru ca modificările politicii să aibă efect pentru utilizatori.** Este posibil să nu puteți efectua imediat modificări la politicile nou create; așteptați 4 ore și încercați să modificați din nou o politică nou creată.

Politicile de întâlnire sunt utilizate pentru a controla caracteristicile disponibile participanților la întâlnire pentru întâlnirile programate de utilizatorii din organizația dvs. Este posibil ca unele caracteristici ale politicilor pentru întâlniri să nu fie implementate încă în centrul de administrare Teams (acestea sunt etichetate cu "în curând" în documentație). În acest caz sau dacă primiți o eroare precum "Nu putem actualiza politica în acest moment, dar încercați din nou mai târziu" din Centrul de administrare Microsoft Teams, vă recomandăm să utilizați PowerShell pentru a crea sau a modifica politicile întâlnirilor Teams. 

Pentru mai multe informații despre politicile de întâlnire, consultați următoarele resurse:

- Pentru a afla despre crearea politicilor, efectuarea de modificări și atribuirea utilizatorilor în politică, consultați Gestionarea politicilor [pentru întâlniri în Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Pentru a face modificări de politică utilizând cmdleturi PowerShell, consultați [Prezentare generală Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Trebuie să utilizați modulul [Skype for Business PowerShell pentru politicile](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) întâlnirii Teams. 
    - Consultați [documentația cmdleturilor *-CsTeamsMeetingPolicy pentru mai](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) multe informații.

