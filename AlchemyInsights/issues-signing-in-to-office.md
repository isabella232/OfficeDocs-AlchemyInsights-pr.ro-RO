---
title: Probleme la conectarea la Microsoft 365 uri
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088048"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Ecran de conectare necompletat în Microsoft 365 aplicații

Pentru a remedia această problemă, încercați următoarele:
- Instalați cele mai recente actualizări [pentru Windows](https://support.microsoft.com/help/4027667/windows-10-update) și [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Resetați opțiunile Internet Explorer: Accesați Instrumente Opțiuni internet Resetare complexă  >    >    >  **Internet Explorer Setări** (rețineți că veți pierde setările particularizate), apoi încercați să vă conectați din Office nou.
- Dezactivați Protecție aplicații Windows Defender (WDAG) sau orice paravan de protecție similar sau program antivirus similar:
    1. În Panoul de control, accesați **Programe**, apoi alegeți **Activare sau Windows a caracteristicilor**.
    2. Dacă Protecție aplicații Windows Defender activat, încercați să-l dezactivare.<br/>
    **Notă:** Poate fi necesar să reporniți computerul.
- Asigurați-vă că insertul Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nu este blocat de nicio aplicație sau de program antivirus/firewall.
- [Goliți Office acreditările](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Windows de acreditări.<br/>
    **Notă:** Căile de registry pentru Office 2016 s-au modificat la 16.0. (De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)

Pentru mai multe informații, consultați Probleme de conectare după actualizarea la [Office 2016 compilarea 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)pe Windows 10 .