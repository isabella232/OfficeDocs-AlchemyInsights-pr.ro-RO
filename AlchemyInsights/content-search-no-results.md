---
title: Căutare conținut fără rezultate
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816860"
---
# <a name="no-results-from-content-searchexports"></a>Niciun rezultat din Căutarea/exporturile de conținut

Problemele cu căutarea/exportul de conținut care nu returnează date pot fi cauzate de un anumit Filtru de securitate de conformitate care a fost configurat de un anumit Administrator și nu îl comunică tuturor administratorilor.

Pentru a rezolva această problemă, verificați dacă există filtre de securitate de conformitate care pot fi cauza acestei probleme:
1. Conectarea la Centrul de securitate și conformitate Powershell
2. Rulați următoarele commandleturi:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organizația $org