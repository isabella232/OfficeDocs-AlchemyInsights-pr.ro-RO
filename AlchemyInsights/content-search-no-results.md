---
title: Căutare conținut niciun rezultat
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680659"
---
# <a name="no-results-from-content-searchexports"></a>Niciun rezultat din căutarea de conținut/exporturi

Probleme cu căutarea de conținut/exporturile care nu returnează date pot fi cauzate de un anumit filtru de securitate de conformitate care a fost configurat de un anumit administrator și nu l-a comunicat tuturor administratorilor.

Pentru a rezolva acest lucru, Verificați dacă există filtre de securitate conformității care pot provoca acest lucru:
1. Conectarea la centrul de securitate și conformitate PowerShell
2. Rulează următorul commandlet:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organizație $org