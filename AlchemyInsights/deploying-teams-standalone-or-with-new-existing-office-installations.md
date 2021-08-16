---
title: Implementarea Teams ca instalare de sistem existentă sau nouă sau Office noi
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
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102214"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Implementarea Teams ca instalare de sistem existentă sau nouă sau Office noi

Microsoft Teams este inclus acum ca  parte a noilor instalări de Aplicații Microsoft 365 pentru întreprindere, Aplicații Microsoft 365 pentru afaceri și Office pentru Mac. Pentru mai multe informații, [consultați Când Microsoft Teams include noile instalări de Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

În plus, începând cu versiunea 1906 din Canalul  Curente, Teams va fi adăugat la instalările existente de Aplicații Microsoft 365 pentru întreprindere (și Aplicații Microsoft 365 pentru afaceri) pe dispozitivele care rulează Windows atunci când actualizați instalarea existentă la cea mai recentă versiune. Pentru mai multe informații, consultați [Ce se întâmplă cu instalările existente ale Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Dacă nu doriți să așteptați această planificare a implementării, puteți implementa Teams [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) ca independent pentru utilizatorii dvs. urmând aceste instrucțiuni sau le puteți spune utilizatorilor să instaleze Teams pentru ei din [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Dacă organizația dvs. nu este gata să implementeze Teams, avem pașii pe [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) care [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) îi puteți urma pentru ***a exclude Teams*** din instalările noi sau existente de Office. Dacă doriți Teams să fie instalat, dar nu doriți ca Teams să pornească automat pentru utilizator după ce este instalat, consultați Împiedicarea ca Microsoft Teams să pornească automat [după instalare.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Pentru a ***dezinstala Teams de*** pe un dispozitiv care rulează Windows, consultați [Dezinstalarea Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Pentru a curăța Microsoft Teams mai multe dispozitive țintă sau utilizatori, consultați [Curățarea implementării Microsoft Teams multiple.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Dacă utilizați computere partajate, servicii desktop la distanță (RDS) sau infrastructura desktop virtuală (VDI), consultați Computere partajate și medii [VDI cu Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Dacă utilizați mai multe Office Mac, consultați Utilizarea [Microsoft Teams pe un Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> După Teams este instalat, se [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) actualizează automat aproximativ la fiecare două săptămâni cu noi caracteristici și actualizări de calitate. 