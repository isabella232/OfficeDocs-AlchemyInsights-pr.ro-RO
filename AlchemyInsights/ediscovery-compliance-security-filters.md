---
title: Nu a fost returnat niciun rezultat în timpul căutării de conținut/export
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727235"
---
# <a name="no-results-returned-during-content-searchexport"></a>Nu a fost returnat niciun rezultat în timpul căutării de conținut/export

Dacă întâmpinați probleme cu următoarele scenarii eDiscovery:

- Căutarea de conținut/exportul nu returnează date sau date neașteptate
- Căutarea sau exportul eDiscovery nu reușește

Acest lucru se poate datora anumitor filtre de securitate conformității care au fost de configurare de către un anumit administrator și nu au fost comunicate către toți administratorii.

Pentru a rezolva acest lucru, Verificați dacă există filtre de securitate conformității care pot provoca aceste probleme:

1. Conectarea la centrul de securitate și conformitate PowerShell
2. Rulează următorul commandlet:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Pentru informații suplimentare despre filtrele de securitate de conformitate, consultați [Filtrarea permisiunilor pentru căutarea de conținut](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
