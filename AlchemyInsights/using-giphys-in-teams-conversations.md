---
title: Utilizarea Giphys în Teams conversații
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323532"
---
# <a name="using-giphys-in-teams-conversations"></a>Utilizarea Giphys în Teams conversații

Accesul giphys Teams chat este activat în mod implicit. Ca administrator, puteți controla dacă Giphys sunt [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) disponibile pentru utilizatori, setând o politică de mesagerie și asigurându-vă că **Utilizați Giphys** în conversații este **On.**

Dacă GIF-urile nu funcționează așa cum vă așteptați în Teams, verificați:

Politica [de mesagerie trebuie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) să permită Giphys. Pentru a verifica utilizând cmdleturi PowerShell:

- Verificați dacă puteți [gestiona Teams cu PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Rulați comanda PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) și verificați dacă **AllowGiphy** este setat la **TRUE.**
- Dacă **AllowGiphy** este setat la **FALSE**, rulați următoarea comandă PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Experiențele conectate opționale](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) trebuie să fie activate pentru a permite accesul la URL-ul Giphy.

**Notă:** dacă aveți mai multe politici de mesagerie Teams configurate pentru entitatea dvs. găzduită, puteți determina identitatea politicii atribuite utilizatorului afectat, folosind comanda PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Selectați TeamsMessagingPolicy.
