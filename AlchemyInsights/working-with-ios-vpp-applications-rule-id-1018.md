---
title: Lucrul cu iOS VPP Applications Regula ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719969"
---
# <a name="working-with-ios-vpp-applications"></a>Lucrul cu iOS VPP Applications

Citiți [Cum se gestionează aplicațiile iOS achiziționate printr-un program de achiziție în volum cu Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) pentru a afla despre caracteristici, constrângeri și pași pentru a utiliza Programul de achiziționare de volum Apple și asistența pentru acesta în Microsoft Intune.
  
 **Probleme comune:** "Am atribuit o aplicație VPP iOS utilizatorilor mei, dar instalarea nu a reușit."
  
- Acest lucru se poate întâmpla dacă un singur simbol VPP este utilizat în mai mulți furnizori de gestionare a dispozitivelor mobile. Token-urile VPP de la Apple pot fi utilizate numai cu un singur furnizor. Dacă ați utilizat un simbol VPP cu mai mulți furnizori, trebuie să încărcați din nou simbolul intune.

- Instalarea poate, de asemenea, nu dacă numărul total de instalări depășește numărul de licențe. Pentru a vizualiza un raport de utilizare pentru licențele dvs., accesați pagina \> **licențe pentru** **aplicații mobile Intune.** Pentru a afla să revendicați licențele utilizate, consultați [acest articol.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
