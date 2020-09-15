---
title: Eroare 4c7 teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700215"
---
# <a name="4c7-error-in-microsoft-teams"></a>eroare 4c7 în Microsoft teams

Această eroare apare deoarece Microsoft teams necesită autentificarea formularelor. Atunci când implementați Active Directory Federation Services (AD FS), autentificarea de formulare nu este activată implicit pentru intranet. Dacă autentificarea integrată Windows nu reușește, vi se solicită să vă conectați utilizând autentificarea formularelor.

Pentru a rezolva această problemă, activați autentificarea formularelor utilizând utilitarul de completare snap-in AD FS Microsoft consolă de gestionare (MMC) pe computerul care conține copia locală a Active Directory. Pentru a proceda astfel, urmați acești pași: 

1. În panoul de navigare, răsfoiți la **politicile de autentificare**.
2. Sub **acțiuni** în panoul de detalii, selectați **Editare autentificare principală globală**.
3. Pe fila **intranet** , selectați **autentificare formulare**.
4. Selectați **OK** (sau **aplicați**).