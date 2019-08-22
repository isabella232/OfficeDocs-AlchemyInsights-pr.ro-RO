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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516791"
---
# <a name="no-results-from-content-searchexports"></a>Nici un rezultat la conţinut căutare/exporturilor

Probleme cu conţinut căutare/exporturile nu reveni orice date se poate datora anumitor filtru de securitate a conformității care a fost de configurare de un Admin specifice şi nu se comunică la toate administratori.

Pentru a rezolva acest lucru, verificaţi pentru a vedea dacă există orice conformitatea filtrele de securitate care poate fi cauza acest lucru:
1. Conecta la securitatea şi conformitatea centrul Powershell
2. Executaţi comenzile următoare:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organizare $org