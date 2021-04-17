---
title: Probleme la conectarea la aplicațiile Microsoft 365
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
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833051"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Ecran de conectare necompletat în aplicațiile Microsoft 365

Pentru a remedia această problemă, încercați următoarele:
- Instalați cele mai recente actualizări [pentru Windows](https://support.microsoft.com/help/4027667/windows-10-update) și [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Resetați opțiunile Internet Explorer: Accesați Instrumente Opțiuni internet - Setări complexe  >    >    >  **de resetare Internet Explorer** (rețineți că veți pierde setările particularizate), apoi încercați din nou să vă conectați la Office.
- Dezactivați Windows Defender Application Guard (WDAG) sau orice program similar de firewall sau antivirus:
    1. În Panoul de control, accesați **Programe**, apoi alegeți **Activare sau dezactivare caracteristici Windows**.
    2. Dacă Windows Defender Application Guard este activat, încercați să-l dezactivare.<br/>
    **Notă:** Poate fi necesar să reporniți computerul.
- Asigurați-vă că insertul Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nu este blocat de nicio aplicație sau de program antivirus/firewall.
- [Goliți acreditările Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Managerul de acreditări Windows.<br/>
    **Notă:** Căile de registry pentru Office 2016 s-au modificat la 16.0. (De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)

Pentru mai multe informații, consultați Probleme de conectare la conectare după actualizarea la [Office 2016, compilarea 16.0.7967 din Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)