---
title: Aplicarea celor mai bune practici pentru interogările complexe de vânătoare
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749546"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Aplicarea celor mai bune practici pentru interogările complexe de vânătoare

Pentru a obține rezultate mai rapid și pentru a evita expirarea în timp ce rulați interogări complexe, aplicați aceste bune practici:

- Atunci când încercați interogări noi, utilizați întotdeauna o limită, pentru a evita să obțineți seturi de rezultate extrem de mari. De asemenea, utilizați `count` pentru a face o evaluare inițială a dimensiunii setului de rezultate.
- Utilizați mai întâi filtrele de timp. În mod ideal, limitați interogările la șapte zile.
- La începutul unei interogări, imediat după filtrul de timp, adăugați filtrele de așteptat pentru a elimina majoritatea datelor.
- Atunci când căutați jetoane complete, utilizați operatorul, `has` mai degrabă decât `contains` .
- Rulează o căutare pe o anumită coloană, mai degrabă decât pe toate coloanele.
- Atunci când vă asociați la tabele, specificați mai întâi tabelul cu mai puține rânduri.
- `project` numai coloanele necesare din tabelele pe care le-ați asociat.

Pentru a afla mai multe, consultați [cele mai bune practici pentru interogarea de vânătoare complexe](https://go.microsoft.com/fwlink/?linkid=2144812).
