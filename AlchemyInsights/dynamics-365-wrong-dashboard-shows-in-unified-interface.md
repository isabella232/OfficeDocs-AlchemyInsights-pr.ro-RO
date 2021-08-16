---
title: Dynamics 365 - afișează un tablou de bord greșit în interfața unificată Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101494"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Un tablou de bord greșit se afișează în interfața unificată Dynamics 365

Există mai multe motive pentru care este posibil să vedeți un alt tablou de bord decât cel așteptat:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Utilizatorul a setat un tablou de bord implicit pentru utilizator 

De obicei, puteți identifica un tablou de bord implicit pentru utilizator dacă butonul **Setare** ca implicit nu se afișează în bara de comenzi a tabloului de bord. Tabloul de bord implicit al utilizatorului va înlocui toate celelalte tablouri de bord implicite, chiar dacă tabloul de bord implicit al utilizatorului nu se află în aplicația curentă.

Utilizați următoarea soluție pentru a anula setarea tabloului de bord implicit.

1. Creați un tablou de bord personal nou.

2. Setați tabloul de bord nou ca utilizator implicit.

3. Ștergeți tabloul de bord.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Tabloul de bord este setat în harta site-ului

Poate că ați setat un tablou de bord implicit al unei organizații selectând un tablou de bord și alegând "Setare ca implicit" sub "Particularizați sistemul". Dar tabloul de bord definit în proiectantul hărții site-ului va avea prioritate în fața acestui tablou de bord, dacă utilizatorul are acces la el.

Pentru ca utilizatorii să vadă tabloul de bord pe care l-ați setat ca organizație implicit, puteți:

* Setarea tabloului de bord în harta site-ului

* Eliminarea accesului la tabloul de bord definit pentru harta site-ului pentru acei utilizatori
