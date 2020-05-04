---
title: Implementarea echipelor ca independent sau cu instalări Office noi sau existente
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: ffa91eaf333792af149feda25f9a377ed591b597
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010230"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Implementarea echipelor ca independent sau cu instalări Office noi sau existente

Microsoft Teams este acum inclus ca parte a ***instalărilor noi*** ale Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business și Office for Mac. Pentru mai multe informații, consultați [Când va începe microsoft Teams să fie inclus ea cu instalările noi de Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

În plus, începând cu versiunea 1906 din Lunar Channel, echipele vor fi ***adăugate la instalările existente*** ale Microsoft 365 Apps for enterprise (și Microsoft 365 Apps for business) pe dispozitive care rulează Windows atunci când actualizați instalarea existentă la cea mai recentă versiune. Pentru mai multe informații, consultați [Ce se întâmplă cu instalările existente de Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Dacă nu doriți să așteptați acest program de lansare, puteți implementa Echipe ca independent pentru utilizatorii dvs., urmând [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)aceste [instrucțiuni](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) sau puteți solicita utilizatorilor să instaleze echipe pentru ei înșiși din .

Dacă organizația nu este pregătită să implementeze Echipe, avem pașii pe care îi puteți urma pentru a ***exclude Echipele*** din instalările [office noi](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) sau [existente.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Dacă doriți ca Echipele să fie instalate, dar nu doriți ca Echipele să pornească automat pentru utilizator după instalare, consultați [Împiedicarea pornirii automată a Echipelor Microsoft după instalare](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Pentru a ***dezinstala Echipe*** de pe un dispozitiv care rulează Windows, consultați [Dezinstalarea Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Pentru a curăța Microsoft Teams de mai multe mașini țintă sau utilizatori, consultați [Implementarea Microsoft Teams curățare](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Dacă utilizați computere partajate, Servicii Desktop la distanță (RDS) sau Virtual Desktop Infrastructure (VDI), consultați [Medii de computer partajat și VDI cu Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Dacă utilizați Office pentru Mac, consultați [instalările Microsoft Teams pe un Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> După instalarea Echipelor, acesta este [actualizat automat](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) aproximativ la fiecare două săptămâni, cu caracteristici noi și actualizări de calitate. 