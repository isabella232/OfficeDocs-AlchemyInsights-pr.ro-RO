---
title: Setările politicii de întâlnire
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627586"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gestionați politicile de întâlnire în Microsoft teams

Politicile de întâlnire sunt utilizate pentru a controla caracteristicile care sunt disponibile pentru a întâlni participanți pentru întâlniri care sunt programate de către utilizatorii din organizația dvs. Este posibil ca unele caracteristici ale politicilor de întâlnire să nu fie implementate în centrul de administrare a echipelor încă (acestea sunt etichetate "în curând" în documentație). În acest caz, sau dacă se obține o eroare de genul "nu putem actualiza politica chiar acum, dar încercați din nou mai târziu" în centrul de administrare Microsoft teams, vă recomandăm să utilizați PowerShell pentru a crea sau modifica echipele de întâlnire politici. 

Pentru mai multe informații despre politicile de întâlnire, consultați următoarele resurse:

- Pentru a afla despre crearea politicilor, efectuarea modificărilor și asocierea utilizatorilor la politică, consultați [gestionarea politicilor de întâlnire în echipe](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Pentru a face modificări de politică utilizând cmdleturi PowerShell, consultați [Prezentare generală a echipelor PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Trebuie să utilizați [Skype pentru afaceri PowerShell modulul](https://www.microsoft.com/download/details.aspx?id=39366) pentru echipele de întâlnire politici. 
    - Examinați [documentația *-csteamsmeetingpolicy cmdlet](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) pentru mai multe informații.

**Notă:** Poate dura până la 24 de ore pentru ca modificările de politică să aibă efect pentru utilizatori. Este posibil să nu puteți modifica imediat politicile nou create; Așteptați 4 ore și încercați să modificați din nou o politică nou creată. Dacă încă întâmpinați probleme, încercați PowerShell.  