---
title: Dynamics 365-greșit tabloul de bord arată în Dynamics 365 interfață unificată
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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36528563"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Greșit tabloul de bord arată în Dynamics 365 interfață unificată

Există mai multe motive pentru care este posibil să vedeți un tablou de bord diferit de cel la care vă așteptați:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Utilizatorul a setat un tablou de bord implicit de utilizator 

De obicei, aveți posibilitatea să identificați un tablou de bord implicit de utilizator este setată dacă butonul **set as default** nu se afișează în bara de comenzi a tabloului de bord. Tabloul de bord implicit de utilizator va suprascrie toate celelalte tablouri de bord implicite, chiar dacă tabloul de bord implicit al utilizatorului nu este în aplicația curentă.

Utilizați următoarea soluție pentru a deseta tabloul de bord implicit.

1. Creați un tablou de bord personal nou.

2. Setați tabloul de bord nou ca implicit de utilizator.

3. Ștergeți tabloul de bord.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Tabloul de bord este setat în Sitemap

Este posibil să fi setat un tablou de bord implicit de organizație selectând un tablou de bord și alegând "setați ca implicit" sub "Particularizare sistem". Dar tabloul de bord definit în proiectantul de Sitemap va avea prioritate față de acest tablou de bord, dacă utilizatorul are acces la acesta.

Pentru ca utilizatorii să vadă tabloul de bord pe care l-ați setat ca implicit al Organizației, puteți fie:

* Setați tabloul de bord în Sitemap

* Eliminați accesul la tabloul de bord definit de Sitemap pentru acei utilizatori
