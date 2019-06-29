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
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364875"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="8c30d-102">Lucrul cu iOS aplicatii VPP</span><span class="sxs-lookup"><span data-stu-id="8c30d-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="8c30d-103">Citiţi [cum să gestioneze aplicaţii iOS achiziţionate printr-un program de volum-cumpărare cu Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) pentru a învăţa despre caracteristici, constrângerile şi măsurile pentru a face uz de programul de cumpărare Apple volumul şi suportul pentru acesta în Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="8c30d-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="8c30d-104">**Probleme comune:** "Am atribuit utilizatorii mei un app de VPP-uri iOS, dar instalarea nu a reuşit."</span><span class="sxs-lookup"><span data-stu-id="8c30d-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="8c30d-105">Acest lucru se poate întâmpla în cazul în care un singur simbol VPP este folosit în mai multe furnizori de management de dispozitiv mobil.</span><span class="sxs-lookup"><span data-stu-id="8c30d-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="8c30d-106">Jetoanele de VPP-uri la Apple pot fi utilizate numai cu un singur furnizor.</span><span class="sxs-lookup"><span data-stu-id="8c30d-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="8c30d-107">Dacă aţi utilizat un tichet de VPP-uri cu mai multe furnizorii de, tu trebuie să re-încărcaţi tichet la Intune.</span><span class="sxs-lookup"><span data-stu-id="8c30d-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="8c30d-108">Instalarea poate eşua, de asemenea, în cazul în care numărul total de instalaţii să depăşească numărul de licenţe.</span><span class="sxs-lookup"><span data-stu-id="8c30d-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="8c30d-109">Pentru a vizualiza un raport de utilizare a licenţelor, du-te la **Intune Mobile apps** \> **App licenţe** filme.</span><span class="sxs-lookup"><span data-stu-id="8c30d-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="8c30d-110">Pentru a afla cum de a recupera licenţe în uz, a se vedea [acest articol.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="8c30d-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
