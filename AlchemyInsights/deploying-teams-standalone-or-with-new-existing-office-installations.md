---
title: Implementarea teams ca independentă sau cu instalări Office noi sau existente
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806771"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Implementarea teams ca independentă sau cu instalări Office noi sau existente

Microsoft teams este inclusă acum ca parte a ***noilor instalări*** de aplicații Microsoft 365 pentru întreprinderi, aplicații Microsoft 365 pentru firme și Office pentru Mac. Pentru mai multe informații, consultați [când va începe Microsoft teams să fie inclusă în instalări noi de Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

În plus, începând cu versiunea 1906 din canalul curent, echipele vor fi ***adăugate la instalările existente*** ale Microsoft 365 Apps pentru întreprinderi (și aplicații Microsoft 365 pentru firme) pe dispozitivele care execută Windows atunci când actualizați instalarea existentă la cea mai recentă versiune. Pentru mai multe informații, consultați [ce se întâmplă cu instalările existente de Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Dacă nu doriți să așteptați pentru acest program de implementare, puteți să implementați teams ca independent pentru utilizatorii dvs., [urmând aceste instrucțiuni](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   sau puteți avea utilizatorii să instaleze teams de la  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Dacă organizația dumneavoastră nu este pregătită să implementeze teams, avem pașii pe care îi puteți face pentru a ***exclude echipele*** din instalări [noi](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) sau [existente](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) de Office. Dacă doriți ca echipele să fie instalate, dar nu doriți ca echipele să pornească automat pentru utilizator după ce este instalat, consultați [împiedicarea pornirii automate a Microsoft teams după instalare](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Pentru a ***dezinstala echipele*** de pe un dispozitiv care execută Windows, consultați [Dezinstalarea Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Pentru a curăța Microsoft teams de la mai multe mașini țintă sau utilizatori, consultați [curățarea implementării Microsoft teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Dacă utilizați computere partajate, Remote Desktop Services (RDS) sau infrastructură desktop virtuală (VDI), consultați [computere partajate și medii VDI cu Microsoft teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Dacă utilizați Office pentru Mac, consultați [instalările Microsoft teams pe un Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> După ce teams este instalat, acesta este [actualizat automat](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) aproximativ la fiecare două săptămâni, cu caracteristici noi și actualizări de calitate. 