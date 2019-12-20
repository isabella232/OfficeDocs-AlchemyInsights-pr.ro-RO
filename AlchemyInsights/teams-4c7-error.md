---
title: Echipele 4C 7 eroare
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796312"
---
# <a name="4c7-error-in-microsoft-teams"></a>eroare 4C 7 în Microsoft teams

Această eroare apare deoarece Microsoft teams necesită autentificarea formularelor. Când implementați consolidare servicii de federalizare Active Directory (AD FS), autentificarea formularelor nu este activată pentru intranet în mod implicit. Dacă autentificarea integrată Windows nu reușește, vi se solicită să faceți sign in utilizând autentificarea formularelor.

Pentru a rezolva această problemă, activați autentificarea formularelor utilizând utilitarul de completare snap-in AD FS Microsoft Management Console (MMC) pe computerul care are copia locală a Active Directory. Pentru a proceda astfel, urmați acești pași: 

1. În panoul de navigare, răsfoiți la **politicile de autentificare**.
2. Sub **acțiuni** în panoul de detalii, selectați **editați autentificarea primară globală**.
3. În fila **intranet** , selectați **autentificarea formularelor**.
4. Selectați **OK** (sau **aplicați**).