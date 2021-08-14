---
title: Aplicați cele mai bune practici pentru interogări complexe de căutare
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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930145"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Aplicați cele mai bune practici pentru interogări complexe de căutare

Pentru a obține rezultate mai rapid și a evita expirarea în timp ce rulați interogări complexe, aplicați aceste bune practici:

- Atunci când încercați interogări noi, utilizați întotdeauna o limită, pentru a evita obținerea unor seturi de rezultate extrem de mari. De asemenea, `count` utilizați pentru a efectua o evaluare inițială a dimensiunii setului de rezultate.
- Utilizați mai întâi filtrele de timp. În mod ideal, limitați interogările la șapte zile.
- La începutul unei interogări, imediat după filtrul de timp, adăugați filtrele așteptate pentru a elimina cea mai mare parte a datelor.
- Atunci când căutați simboluri complete, utilizați `has` operatorul în loc de `contains` .
- Rulați o căutare pe o anumită coloană, nu în toate coloanele.
- Când vă alăturați tabelelor, specificați mai întâi tabelul cu mai puține rânduri.
- `project` numai coloanele necesare din tabelele pe care le-ați unit.

Pentru a afla mai multe, consultați Cele mai bune practici [pentru interogarea de căutare complexă.](https://go.microsoft.com/fwlink/?linkid=2144812)
