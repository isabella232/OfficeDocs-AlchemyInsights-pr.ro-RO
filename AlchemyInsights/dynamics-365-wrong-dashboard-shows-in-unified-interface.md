---
title: Dynamics 365 - tabloul de bord greşit arată în interfaţă unificată Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528563"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Tabloul de bord greşit arată în interfaţă unificată Dynamics 365

Există mai multe motive de ce pot vedea un tablou de bord diferite decât cea pe care aţi aştepta:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Utilizatorul a stabilit un tablou de bord utilizator implicit 

De obicei poate identifica un utilizator implicit tabloul de bord este situat în cazul în care butonul **Setat ca implicit** nu arată în bara de comenzi tabloul de bord. Tabloul de bord utilizator implicit va suprascrie toate alte dashboards implicit, chiar dacă utilizatorul implicit tabloul de bord nu este în app curent.

Utilizaţi următoarele workaround pentru a demarca implicit tabloul de bord.

1. Creați un nou tablou de bord personale.

2. Setaţi ca nou tablou de bord utilizator implicit.

3. Şterge acest tablou de bord.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Tabloul de bord este situat în sitemap

Poate aţi setat o organizaţie implicit tabloul de bord prin selectarea un tablou de bord şi alegerea 'Setat ca Default' sub 'Particularizarea sistemului'. Dar tabloul de bord definite în sitemap proiectantul vor avea prioritate peste acest tablou de bord, în cazul în care utilizatorul are acces la aceasta.

Pentru ca utilizatorii vedea tabloul de bord pe care aţi setat ca implicit organizaţie, aveţi posibilitatea să fie:

* Stabilit că tabloul de bord în sitemap

* Elimina accesul la tabloul de bord sitemap definite pentru acei utilizatori
