---
title: Lucrul cu iOS VPP aplicaţii regula Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29485411"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="441b0-102">Lucrul cu iOS aplicatii VPP</span><span class="sxs-lookup"><span data-stu-id="441b0-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="441b0-103">Citiţi [cum să gestioneze aplicaţii iOS achiziţionate printr-un program de volum-cumpărare cu Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) pentru a învăţa despre caracteristici, constrângerile şi măsurile pentru a face uz de programul de cumpărare Apple volumul şi suportul pentru acesta în Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="441b0-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="441b0-104">**Probleme comune:** "Am atribuit utilizatorii mei un app de VPP-uri iOS, dar instalarea nu a reuşit."</span><span class="sxs-lookup"><span data-stu-id="441b0-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="441b0-p101">Acest lucru se poate întâmpla în cazul în care un singur simbol VPP este folosit în mai multe furnizori de management de dispozitiv mobil. Jetoanele de VPP-uri la Apple pot fi utilizate numai cu un singur furnizor. Dacă aţi utilizat un tichet de VPP-uri cu mai multe furnizorii de, tu trebuie să re-încărcaţi tichet la Intune.</span><span class="sxs-lookup"><span data-stu-id="441b0-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="441b0-p102">Instalarea poate eşua, de asemenea, în cazul în care numărul total de instalaţii să depăşească numărul de licenţe. Pentru a vizualiza un raport de utilizare a licenţelor, du-te la **Intune Mobile apps** \> **App licenţe** filme. Pentru a afla cum de a recupera licenţe în uz, a se vedea [acest articol.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="441b0-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

