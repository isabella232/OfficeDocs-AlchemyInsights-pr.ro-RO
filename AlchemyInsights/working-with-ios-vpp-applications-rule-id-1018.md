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
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="08ae4-102">Lucrul cu iOS VPP Applications</span><span class="sxs-lookup"><span data-stu-id="08ae4-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="08ae4-103">Citiți [Cum se gestionează aplicațiile iOS achiziționate printr-un program de achiziție în volum cu Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) pentru a afla despre caracteristici, constrângeri și pași pentru a utiliza Programul de achiziționare de volum Apple și asistența pentru acesta în Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="08ae4-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="08ae4-104">**Probleme comune:** "Am atribuit o aplicație VPP iOS utilizatorilor mei, dar instalarea nu a reușit."</span><span class="sxs-lookup"><span data-stu-id="08ae4-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="08ae4-105">Acest lucru se poate întâmpla dacă un singur simbol VPP este utilizat în mai mulți furnizori de gestionare a dispozitivelor mobile.</span><span class="sxs-lookup"><span data-stu-id="08ae4-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="08ae4-106">Token-urile VPP de la Apple pot fi utilizate numai cu un singur furnizor.</span><span class="sxs-lookup"><span data-stu-id="08ae4-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="08ae4-107">Dacă ați utilizat un simbol VPP cu mai mulți furnizori, trebuie să încărcați din nou simbolul intune.</span><span class="sxs-lookup"><span data-stu-id="08ae4-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="08ae4-108">Instalarea poate, de asemenea, nu dacă numărul total de instalări depășește numărul de licențe.</span><span class="sxs-lookup"><span data-stu-id="08ae4-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="08ae4-109">Pentru a vizualiza un raport de utilizare pentru licențele dvs., accesați pagina \> **licențe pentru** **aplicații mobile Intune.**</span><span class="sxs-lookup"><span data-stu-id="08ae4-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="08ae4-110">Pentru a afla să revendicați licențele utilizate, consultați [acest articol.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="08ae4-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
