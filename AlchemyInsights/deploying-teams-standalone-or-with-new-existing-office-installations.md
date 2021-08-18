---
title: Implementarea Teams ca instalări de aplicații noi sau existente, Office noi
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
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320134"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Implementarea Teams ca instalări de aplicații noi sau existente, Office noi

Microsoft Teams este inclus acum ca  parte a noilor instalări de Aplicații Microsoft 365 pentru întreprindere, de Aplicații Microsoft 365 pentru afaceri de computer Office pentru Mac. Pentru mai multe informații, [consultați Când Microsoft Teams include noile instalări de Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

În plus, începând cu versiunea 1906 din Canalul  Curente, Teams va fi adăugat la instalările existente de Aplicații Microsoft 365 pentru întreprindere (și Aplicații Microsoft 365 pentru afaceri) pe dispozitivele care rulează Windows atunci când actualizați instalarea existentă la cea mai recentă versiune. Pentru mai multe informații, consultați [Ce se întâmplă cu instalările existente ale Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Notă:** Dacă nu doriți să așteptați această planificare a implementării, puteți implementa Teams [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) ca independent pentru utilizatorii dvs. urmând aceste instrucțiuni sau le puteți spune utilizatorilor să instaleze Teams pentru ei din [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Dacă organizația dvs. nu este gata să implementeze Teams, avem pașii pe [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) care [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) îi puteți urma pentru a ***exclude*** Teams din instalările noi sau existente de Office. Dacă doriți Teams să fie instalat, dar nu doriți ca Teams să pornească automat pentru utilizator după ce este instalat, consultați Împiedicarea ca Microsoft Teams să pornească automat [după instalare.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Pentru a ***dezinstala Teams*** de pe un dispozitiv care rulează Windows, consultați [Dezinstalarea Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Pentru a curăța Microsoft Teams mai multe dispozitive țintă sau utilizatori, consultați [Curățarea implementării Microsoft Teams multiple.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Dacă utilizați computere partajate, servicii desktop la distanță (RDS) sau infrastructura desktop virtuală (VDI), consultați Computere partajate și medii [VDI cu Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Dacă utilizați mai multe Office Mac, consultați Utilizarea [Microsoft Teams pe un Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**Notă:** după Teams este instalat, [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) se actualizează automat la fiecare două săptămâni, aproximativ, cu noi caracteristici și actualizări de calitate. 