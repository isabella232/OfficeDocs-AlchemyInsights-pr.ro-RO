---
title: Conţinut fără rezultate
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800538"
---
# <a name="no-results-from-content-searchexports"></a>Nici un rezultat la conţinut căutare/exporturilor

Probleme cu conţinut căutare/exporturile nu reveni orice date se poate datora anumitor filtru de securitate a conformității care a fost de configurare de un Admin specifice şi nu se comunică la toate administratori.

Pentru a rezolva acest lucru, verificaţi pentru a vedea dacă există orice conformitatea filtrele de securitate care poate fi cauza acest lucru:
1. Conecta la securitatea şi conformitatea centrul Powershell
2. Executaţi comenzile următoare:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organizare $org