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
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680325"
---
# <a name="no-results-returned-during-content-searchexport"></a>Nu a fost returnat niciun rezultat în timpul căutării de conținut/export

Dacă întâmpinați probleme cu următoarele scenarii eDiscovery:

- Căutarea de conținut/exportul nu returnează date sau date neașteptate
- Căutarea sau exportul eDiscovery nu reușește

Acest lucru poate fi cauzat din cauza anumitor filtre de securitate conformității care au fost de configurare de către un anumit administrator și nu au fost comunicate către toți administratorii.

Pentru a rezolva acest lucru, Verificați dacă există filtre de securitate conformității care pot provoca aceste probleme:

1. Conectarea la centrul de securitate și conformitate PowerShell
2. Rulează următorul commandlet:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Pentru informații suplimentare despre filtrele de securitate de conformitate, consultați [Filtrarea permisiunilor pentru căutarea de conținut](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
