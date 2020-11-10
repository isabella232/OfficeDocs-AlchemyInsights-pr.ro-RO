---
title: Utilizarea Giphy în conversațiile teams
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982580"
---
# <a name="using-giphys-in-teams-conversations"></a>Utilizarea Giphy în conversațiile teams

Accesul giphy în teams chat este activat în mod implicit. Ca administrator, puteți să controlați dacă Giphy sunt disponibili pentru utilizatori [setând o politică de mesagerie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) și asigurându-vă că **Utilizați giphy în conversații** este **activată**.

Dacă GIF-urile nu funcționează așa cum vă așteptați în conversațiile teams, verificați:

[Politica de mesagerie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) trebuie să permită giphy. Pentru a verifica dacă utilizați cmdleturi PowerShell:

- Verificați dacă puteți [gestiona teams cu PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Executarea comenzii PowerShell [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) și verificați dacă **AllowGiphy** este setată la **True**.
- Dacă **AllowGiphy** este setată la **false** , rulează următorul set de comenzi PowerShell [-CsTeamsMessagingPolicy-identity global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Experiențele conectate opționale](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) trebuie activate pentru a permite accesul la adresa URL Giphy.

> [!NOTE]
> Dacă aveți mai multe politici de mesagerie pentru echipe configurate pentru entitatea găzduită, puteți determina identitatea politicii atribuite utilizatorului afectat cu comanda PowerShell [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Selectați TeamsMessagingPolicy.
