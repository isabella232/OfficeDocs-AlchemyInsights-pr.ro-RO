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
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117100"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Ce se poate face dacă caracteristicile Azure nu funcționează corect în Microsoft Edge

Microsoft Edge are probleme [cunoscute care](https://go.microsoft.com/fwlink/?linkid=2140608) sunt legate de zonele de securitate și pot afecta modul în care utilizatorii Azure se conectează la centrul Windows de administrare. Dacă aveți probleme la utilizarea caracteristicilor Azure cu Microsoft Edge, încercați acești pași:

1. În meniul **Start,** căutați Opțiuni **Internet și** selectați-l.
2. În caseta **de** dialog Proprietăți internet, accesați **fila** Securitate.
3. Selectați zona **Site-uri** de încredere, apoi selectați **butonul Site-uri.**
4. În caseta de dialog **Site-uri** de încredere, adăugați atât URL-ul gateway-ului, cât [https://login.microsoftonline.com](https://login.microsoftonline.com) și , apoi [https://login.live.com](https://login.live.com) selectați **Închidere**.
5. În caseta de dialog **Proprietăți** internet, accesați fila **Confidențialitate.**
6. În **secțiunea Blocarea ferestrelor pop-up,** **selectați Setări**. În caseta de dialog care se deschide, adăugați atât URL-ul gateway-ului, cât [https://login.microsoftonline.com](https://login.microsoftonline.com) și [https://login.live.com](https://login.live.com) , apoi selectați **Închidere**.
