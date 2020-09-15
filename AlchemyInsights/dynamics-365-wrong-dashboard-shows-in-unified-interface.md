---
title: Dinamica 365-afișează un tablou de bord incorect în interfața unificată Dynamics 365
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
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711287"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Afișează un tablou de bord greșit în interfața unificată Dynamics 365

Există mai multe motive pentru care este posibil să vedeți un tablou de bord diferit de cel la care vă așteptați:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Utilizatorul a setat un tablou de bord implicit pentru utilizator 

De obicei, puteți identifica un tablou de bord implicit pentru utilizator este setat dacă butonul **Stabilire ca implicit** nu se afișează în bara de comenzi tablou de bord. Tabloul de bord implicit pentru utilizator va anula toate celelalte tablouri de bord implicite, chiar dacă tabloul de bord implicit al utilizatorului nu se află în aplicația curentă.

Utilizați următoarea soluție pentru a-i unse tabloul de bord implicit.

1. Creați un tablou de bord personal nou.

2. Setați tabloul de bord nou ca implicit pentru utilizator.

3. Ștergeți tabloul de bord.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Tabloul de bord este setat în Sitemap

Este posibil să fi setat un tablou de bord implicit pentru organizație selectând un tablou de bord și alegând "stabilire ca implicit" sub "Particularizare sistem". Dar tabloul de bord definit în proiectantul Sitemap-urilor va prevala asupra acestui tablou de bord, dacă utilizatorul are acces la acesta.

Pentru ca utilizatorii să vadă tabloul de bord pe care l-ați setat ca implicit al Organizației, puteți fie:

* Setarea tabloului de bord în Sitemap

* Eliminarea accesului la tabloul de bord definit al Sitemap pentru acei utilizatori
