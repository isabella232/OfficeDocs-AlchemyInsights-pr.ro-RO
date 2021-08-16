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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058014"
---
# <a name="no-results-from-content-searchexports"></a>Niciun rezultat din Căutarea/exporturile de conținut

Problemele cu căutarea/exportul de conținut care nu returnează date pot fi cauzate de un anumit Filtru de securitate de conformitate care a fost configurat de un anumit Administrator și nu îl comunică tuturor administratorilor.

Pentru a rezolva această problemă, verificați dacă există filtre de securitate de conformitate care pot fi cauza acestei probleme:
1. Conectare powershell către Centrul de securitate și conformitate
2. Rulați următoarele commandleturi:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organizația $org