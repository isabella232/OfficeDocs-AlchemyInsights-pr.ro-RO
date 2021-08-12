---
title: Ce se poate face dacă caracteristicile Azure nu funcționează corect în Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812876"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Ce se poate face dacă caracteristicile Azure nu funcționează corect în Microsoft Edge

Microsoft Edge probleme cunoscute legate de zonele de securitate care pot afecta modul în care utilizatorii Azure se conectează la Windows de administrare. Pentru mai multe informații, consultați [Probleme cunoscute în Edge.](https://go.microsoft.com/fwlink/?linkid=2140608) Dacă aveți probleme la utilizarea caracteristicilor Azure cu Microsoft Edge, încercați următoarele:

1. Pe fila meniul Start, în bara **Căutare,** tastați **Opțiuni internet**, apoi selectați-l.
1. În **Proprietăți Internet**, selectați **fila** Securitate.
1. Selectați **Site-uri** de încredere , apoi selectați **Site-uri**.
1. Adăugați atât URL-ul gateway-ului, cât <https://login.microsoftonline.com> și și , apoi <https://login.live.com> selectați **Închidere**.
1. În **Proprietăți Internet,** selectați **fila Confidențialitate.**
1. În secțiunea Blocarea ferestrelor pop-up, **selectați Setări**. Adăugați atât URL-ul gateway-ului, cât <https://login.microsoftonline.com> <https://login.live.com> și , apoi selectați **Închidere**.