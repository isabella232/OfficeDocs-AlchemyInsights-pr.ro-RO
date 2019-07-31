---
title: Probleme de sign in la Office apps
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938311"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Semn-înăuntru ecran gol în Office apps

Pentru a remedia această problemă, încercaţi următoarele:
- Instalaţi cele mai recente actualizări pentru [Windows](https://support.microsoft.com/help/4027667/windows-10-update) si [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Reiniţializaţi Internet Explorer opţiuni: Du-te la **Instrumente** > **Opţiuni Internet** > **Advanced** > **Reinițializare setări Internet Explorer** (Notă de faptul că veţi pierde setările particularizate), şi apoi încercaţi conectarea la biroul din nou.
- Dezactivează Windows Defender cerere Garda (WDAG) sau orice program firewall sau anti-virus similar:
    1. În panoul de Control, du-te la **programe**, şi apoi alegeţi **Nap Ferestre features on sau off**.
    2. În cazul în care Garda de aplicaţie Windows Defender este activat, încercaţi să dezactivaţi-l.<br/>
    **Notă:** Trebuie să reporniţi computerul.
- Asiguraţi-vă că Microsoft.AAD.BrokerPlugin [Dai WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nu este blocat de vreo aplicaţie sau un program firewall/anti-anti-virus.
- [Acreditări clar Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Windows Credential Manager.<br/>
    **Notă:** Căi de registry pentru Office 2016 s-au schimbat la 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Pentru informaţii suplimentare, consultaţi [probleme de conexiune în semn-înăuntru după update la Office 2016 construi 16.0.7967 pe Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).