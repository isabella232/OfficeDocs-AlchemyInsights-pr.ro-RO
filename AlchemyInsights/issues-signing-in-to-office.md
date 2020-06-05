---
title: Probleme la conectarea la aplicațiile Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579913"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Ecran de conectare gol în aplicațiile Microsoft 365

Pentru a remedia această problemă, încercați următoarele:
- Instalați cele mai recente actualizări pentru [Windows](https://support.microsoft.com/help/4027667/windows-10-update) și [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Reinițializați opțiunile Internet Explorer: Accesați **Instrumente**  >  **Opțiuni Internet**  >  **Reinițializare avansată**setări Internet  >  **Explorer** (rețineți că veți pierde setările particularizate), apoi încercați din nou să vă conectați la Office.
- Dezactivați Windows Defender Application Guard (WDAG) sau orice firewall similare sau anti-virus program:
    1. În Panoul de control, accesați **Programe**, apoi **alegeți Activare sau dezactivare caracteristici Windows**.
    2. Dacă este activată Garda de aplicație Windows Defender, încercați să o dezactivați.<br/>
    **Notã:** Poate fi necesar să reporniți computerul.
- Asigurați-vă că Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nu este blocat de orice aplicație sau firewall /anti-virus program.
- [Goliți acreditările Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Windows Credential Manager.<br/>
    **Notã:** Căile de registry pentru Office 2016 s-au modificat la 16.0. (De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)

Pentru mai multe informații, consultați [Probleme de conexiune în conectare după actualizarea la Office 2016 build 16.0.7967 pe Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).