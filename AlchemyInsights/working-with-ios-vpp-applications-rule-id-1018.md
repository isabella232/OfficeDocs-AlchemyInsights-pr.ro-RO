---
title: Lucrul cu aplicațiile VPP pentru iOS regulă ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688958"
---
# <a name="working-with-ios-vpp-applications"></a>Lucrul cu aplicațiile VPP pentru iOS

Citiți [cum să gestionați aplicațiile iOS achiziționate printr-un program de achiziționare de volum cu Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) pentru a afla despre caracteristicile, restricțiile și pașii pentru a face uz de programul de achiziții în volum Apple și de suportul pentru acesta în Microsoft Intune.
  
 **Probleme comune:** "Am atribuit o aplicație de iOS VPP utilizatorilor mei, dar instalarea nu a reușit."
  
- Acest lucru se poate întâmpla dacă un singur simbol VPP este utilizat pe mai mulți furnizori de gestionare a dispozitivelor mobile. Simbolurile VPP de la Apple pot fi utilizate doar cu un singur furnizor. Dacă ați utilizat un token VPP cu mai mulți furnizori, trebuie să încărcați din nou simbolul în Intune.

- De asemenea, instalarea poate să nu reușească dacă numărul total de instalări depășește numărul de licențe. Pentru a vizualiza un raport de utilizare pentru licențele dvs. **Intune Mobile apps** , accesați pagina de \> **licențe** pentru aplicațiile mobile din Intune. Pentru a afla cum să revendicați licențele în uz, consultați [acest articol.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
