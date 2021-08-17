---
title: Lucrul cu ID-ul regulii de aplicații vPP iOS 1018
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
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083026"
---
# <a name="working-with-ios-vpp-applications"></a>Lucrul cu aplicațiile VPP iOS

Citiți Cum se gestionează aplicațiile iOS achiziționate [printr-un program](https://docs.microsoft.com/intune/vpp-apps-ios) de achiziții în volum cu Microsoft Intune pentru a afla despre caracteristicile, restricțiile și pașii pentru utilizarea Programului de achiziționare în volum Apple și despre suportul pentru acesta în Microsoft Intune.
  
 **Probleme comune:** "Am atribuit o aplicație VPP iOS utilizatorilor mei, dar instalarea nu a reușit."
  
- Acest lucru se poate întâmpla dacă un singur token VPP este utilizat la mai mulți furnizori de gestionare a dispozitivelor mobile. Simbolurile VPP de la Apple pot fi utilizate doar cu un singur furnizor. Dacă aveți un token VPP cu mai mulți furnizori, trebuie să încărcați din nou simbolul în Intune.

- Instalarea poate să nu reușească și dacă numărul total de instalări depășește numărul de licențe. Pentru a vizualiza un raport de utilizare pentru licențele dvs., accesați **pagina Licențe de aplicații mobile Intune.** \>  Pentru a afla cum să recuperați licențele în uz, consultați [acest articol.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
