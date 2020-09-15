---
title: Probleme la conectarea la aplicațiile Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695299"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Ecran de conectare necompletat în aplicațiile Microsoft 365

Pentru a remedia această problemă, încercați următoarele:
- Instalați cele mai recente actualizări pentru [Windows](https://support.microsoft.com/help/4027667/windows-10-update) și [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Reinițializarea opțiunilor Internet Explorer: accesați **Instrumente**  >  **Opțiuni Internet**  >  **Advanced**  >  **reinițializați setările Internet Explorer** (rețineți că veți pierde setările particularizate), apoi încercați din nou să vă conectați la Office.
- Dezactivați Garda de aplicații Windows Defender (WDAG) sau orice alt program de firewall sau antivirus similar:
    1. În panoul de control, accesați **programe**, apoi alegeți **Activare sau dezactivare caracteristici Windows**.
    2. Dacă Garda de aplicație Windows Defender este activată, încercați să o dezactivați.<br/>
    **Notă:** Poate fi necesar să reporniți computerul.
- Asigurați-vă că [insertul](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. aad. BROKERPLUGIN Dan WAM nu este blocat de nicio aplicație sau de un program firewall/antivirus.
- [Debifați acreditările Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând managerul de acreditări Windows.<br/>
    **Notă:** Căile de registry pentru Office 2016 s-au modificat la 16,0. (De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)

Pentru mai multe informații, consultați [probleme de conexiune în conectarea după actualizare la Office 2016 Build 16.0.7967 pe Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).