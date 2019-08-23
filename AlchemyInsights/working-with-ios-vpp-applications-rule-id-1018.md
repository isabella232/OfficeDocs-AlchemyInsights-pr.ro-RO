---
title: Lucrul cu iOS VPP aplicaţii regula Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558017"
---
# <a name="working-with-ios-vpp-applications"></a>Lucrul cu iOS aplicatii VPP

Citiţi [cum să gestioneze aplicaţii iOS achiziţionate printr-un program de volum-cumpărare cu Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) pentru a învăţa despre caracteristici, constrângerile şi măsurile pentru a face uz de programul de cumpărare Apple volumul şi suportul pentru acesta în Microsoft Intune.
  
 **Probleme comune:** "Am atribuit utilizatorii mei un app de VPP-uri iOS, dar instalarea nu a reuşit."
  
- Acest lucru se poate întâmpla în cazul în care un singur simbol VPP este folosit în mai multe furnizori de management de dispozitiv mobil. Jetoanele de VPP-uri la Apple pot fi utilizate numai cu un singur furnizor. Dacă aţi utilizat un tichet de VPP-uri cu mai multe furnizorii de, tu trebuie să re-încărcaţi tichet la Intune.

- Instalarea poate eşua, de asemenea, în cazul în care numărul total de instalaţii să depăşească numărul de licenţe. Pentru a vizualiza un raport de utilizare a licenţelor, du-te la **Intune Mobile apps** \> **App licenţe** filme. Pentru a afla cum de a recupera licenţe în uz, a se vedea [acest articol.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
