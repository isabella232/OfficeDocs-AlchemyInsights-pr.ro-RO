---
title: Gestionarea înregistrării webinar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793910"
---
# <a name="manage-webinar-registration"></a>Gestionarea înregistrării webinar

Puteți gestiona persoanele care se pot înregistra pentru Teams webinars, utilizând Teams powershell. Pentru a Teams Powershell, consultați [Teams PowerShell.](/microsoftteams/teams-powershell-install) 

În mod implicit, *WhoCanRegister* este activat și setat la **EveryoneInCompany**. Pentru a permite înregistrării tuturor utilizatorilor anonimi, trebuie să setați politica de întâlnire **la Oricine,** utilizând comanda Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Notă:** dacă asocierea anonimă este dezactivată în setările întâlnirii, utilizatorii anonimi nu se pot alătura la webinarii. Pentru a afla mai multe și a activa această setare, [consultați Gestionarea setărilor întâlnirii din Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Dacă doriți să dezactivați înregistrarea întâlnirilor, *setați AllowMeetingRegistration* la **False**.

Pentru a afla mai multe despre configurarea cine se poate înregistra pentru webinarii, consultați [Configurarea cine se poate înregistra pentru webinarii.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Pentru mai multe informații despre setările pentru Liste Microsoft, consultați [Controlați setările pentru Liste Microsoft.](/sharepoint/control-lists)
