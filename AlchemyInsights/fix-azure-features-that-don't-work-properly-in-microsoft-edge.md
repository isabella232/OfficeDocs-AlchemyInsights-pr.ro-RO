---
title: Ce se poate face dacă caracteristicile Azure nu funcționează corect în Microsoft Edge
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583785"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Ce se poate face dacă caracteristicile Azure nu funcționează corect în Microsoft Edge

Microsoft Edge are [probleme cunoscute](https://go.microsoft.com/fwlink/?linkid=2140608) legate de zonele de securitate și pot afecta modul în care utilizatorii Azure se conectează la centrul de administrare Windows. Dacă întâmpinați probleme la utilizarea caracteristicilor Azure cu Microsoft Edge, încercați următorii pași:

1. În meniul **Start** , căutați **Opțiuni Internet** și selectați-l.
2. În caseta de dialog **Proprietăți Internet** , accesați fila **Securitate** .
3. Selectați zona **site-uri de încredere** , apoi selectați butonul **site-uri** .
4. În caseta de dialog **site-uri de încredere** , adăugați adresa URL a gateway-ului, precum [https://login.microsoftonline.com](https://login.microsoftonline.com) și [https://login.live.com](https://login.live.com) , apoi selectați **Închidere**.
5. În caseta de dialog **Proprietăți Internet** , accesați fila **confidențialitate** .
6. În secțiunea **Blocare ferestre pop-up** , selectați **Setări**. În caseta de dialog care se deschide, adăugați adresa URL a gateway-ului, precum [https://login.microsoftonline.com](https://login.microsoftonline.com) și [https://login.live.com](https://login.live.com) , apoi selectați **Închidere**.
