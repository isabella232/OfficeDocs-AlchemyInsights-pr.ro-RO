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
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925177"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gestionarea politicilor pentru întâlniri în Microsoft Teams

**Notă: poate dura până la 24 de ore pentru ca modificările politicii să aibă efect pentru utilizatori.** Este posibil să nu puteți efectua imediat modificări la politicile nou create; așteptați 4 ore și încercați să modificați din nou o politică nou creată.

Politicile de întâlnire sunt utilizate pentru a controla caracteristicile disponibile participanților la întâlnire pentru întâlnirile programate de utilizatorii din organizația dvs. Unele caracteristici ale politicilor pentru întâlniri pot să nu fie implementate încă în centrul de administrare Teams (acestea sunt etichetate cu "în curând" în documentație). În acest caz sau dacă primiți o eroare precum "Nu putem actualiza politica momentan, dar încercați din nou mai târziu" din centrul de administrare Microsoft Teams, vă recomandăm să utilizați PowerShell pentru a crea sau a modifica politicile de întâlnire Teams. 

Pentru mai multe informații despre politicile de întâlnire, consultați următoarele resurse:

- Pentru a afla despre crearea politicilor, efectuarea de modificări și atribuirea de utilizatori la politică, consultați Gestionarea politicilor [pentru întâlniri în Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Pentru a face modificări de politică utilizând cmdleturi PowerShell, consultați [Teams Prezentare generală PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Trebuie să utilizați modulul [Skype for Business PowerShell pentru a Teams](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) pentru întâlniri. 
    - Consultați [documentația cmdleturilor *-CsTeamsMeetingPolicy pentru mai](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) multe informații.

