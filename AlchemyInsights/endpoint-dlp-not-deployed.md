---
title: DLP-ul de punct final nu este implementat pe dispozitivul utilizatorului
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731865"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>DLP-ul de punct final nu este implementat pe dispozitivul utilizatorului

Dacă setarea de prevenire a pierderii datelor punct final (DLP) nu s-a aplicat pentru dispozitivul unui utilizator, confirmați că îndepliniți aceste cerințe:

- Windows 10 1809 sau o versiune mai recentă, este instalată pe dispozitiv.
- Este instalată versiunea 4.18.2009.7 a clientului antimalware versiunea 4.18.2009.7 sau o versiune mai recentă.
- Dispozitivul este **unul dintre** următoarele:
    
    - Azure Active Directory (Azure AD) unit
    - Hibride Azure AD joined
    - AAD înregistrat

- Pentru a impune acțiuni de politică, asigurați-Chromium microsoft Chromium Microsoft Edge este instalat pe dispozitivul punct final.

Pentru cerințe suplimentare pentru implementarea DLP pentru punctul final, consultați Începeți [lucrul cu prevenirea pierderii datelor pentru punctul final.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)