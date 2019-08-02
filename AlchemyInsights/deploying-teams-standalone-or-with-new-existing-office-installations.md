---
title: Implementarea echipe ca independent sau cu instalatii de birou noi sau existente
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054242"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Implementarea echipe ca independent sau cu instalatii de birou noi sau existente

Teams Microsoft este acum inclus ca parte din ***noile instalări*** Office 365 ProPlus, Office 365 Business si Office pentru Mac. Pentru informaţii suplimentare, consultaţi [când va începe Microsoft Teams fiind incluse cu noile instalări de birou?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

În plus, începând cu versiunea 1906 în lunar canalului, echipe va fi ***adăugat la instalațiile existente*** de Office 365 ProPlus (şi Office 365 Business) pe dispozitivele ce ruleaza Windows atunci când vă actualiza instalarea existentă la ultima versiune. Pentru informaţii suplimentare, consultaţi [ce despre instalaţiile existente de birou?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Dacă nu doriţi să aşteptaţi pentru acest program de rollout, se poate implementa pe echipe ca independent pentru utilizatorii dvs., urmând [aceste instrucţiuni](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) sau puteţi avea utilizatorii instala echipe de la sine din [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

În cazul în care organizaţia nu este gata pentru a implementa echipe, avem măsuri puteţi lua pentru a ***exclude echipe*** din instalaţiile [noi](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) sau [existente](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) de birou. Daca vrei echipe sa fie instalat, dar nu doresc să pornească automat pentru utilizator după ce este instalat, se [Împiedică Microsoft echipe începând automat dupa instalare](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Pentru a ***dezinstala echipe*** de pe un dispozitiv care execută Windows, a se vedea [Uninstall Microsoft echipe](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Pentru curăţire Microsoft Teams din mai multe maşini de ţintă sau utilizatori, vedea [echipele Microsoft implementare curat](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

În cazul în care utilizaţi computere partajate, Remote Desktop servicii (RDS), sau Virtual Desktop infrastructură (VDI), vedea [Shared computer şi VDI medii cu echipele de Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Dacă utilizaţi Office pentru Mac, vedea [instalări Microsoft echipe pe un Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> După ce este instalat echipe, este [actualizat automat](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) aproximativ fiecare două săptămâni cu caracteristici noi şi actualizări de calitate. 