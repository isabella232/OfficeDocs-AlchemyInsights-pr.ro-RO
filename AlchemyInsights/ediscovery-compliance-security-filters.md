---
title: Nu s-au returnat rezultate în timpul căutării/exportului de conținut
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101278"
---
# <a name="no-results-returned-during-content-searchexport"></a>Nu s-au returnat rezultate în timpul căutării/exportului de conținut

Dacă aveți probleme cu următoarele scenarii de descoperire a informațiilor electronic:

- Căutarea/Exportul conținutului nu returnează date sau date neașteptate
- Căutarea sau exportul eDiscovery nu reușește

Acest lucru poate fi cauzat de anumite filtre de securitate de conformitate care au fost configurate de un anumit administrator și nu au fost comunicate tuturor administratorilor.

Pentru a rezolva această problemă, verificați dacă există filtre de securitate de conformitate care pot fi cauza acestor probleme:

1. Conectare powershell către Centrul de securitate și conformitate
2. Rulați următoarele commandleturi:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Pentru informații suplimentare despre filtrele de securitate a conformității, [consultați Filtrarea permisiunilor pentru căutarea conținutului](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
