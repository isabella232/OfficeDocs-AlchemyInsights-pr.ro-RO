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
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="94124-102">Lucrul cu aplicațiile VPP pentru iOS</span><span class="sxs-lookup"><span data-stu-id="94124-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="94124-103">Citiți [cum să gestionați aplicațiile iOS achiziționate printr-un program de achiziționare de volum cu Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) pentru a afla despre caracteristicile, restricțiile și pașii pentru a face uz de programul de achiziții în volum Apple și de suportul pentru acesta în Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="94124-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="94124-104">**Probleme comune:** "Am atribuit o aplicație de iOS VPP utilizatorilor mei, dar instalarea nu a reușit."</span><span class="sxs-lookup"><span data-stu-id="94124-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="94124-105">Acest lucru se poate întâmpla dacă un singur simbol VPP este utilizat pe mai mulți furnizori de gestionare a dispozitivelor mobile.</span><span class="sxs-lookup"><span data-stu-id="94124-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="94124-106">Simbolurile VPP de la Apple pot fi utilizate doar cu un singur furnizor.</span><span class="sxs-lookup"><span data-stu-id="94124-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="94124-107">Dacă ați utilizat un token VPP cu mai mulți furnizori, trebuie să încărcați din nou simbolul în Intune.</span><span class="sxs-lookup"><span data-stu-id="94124-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="94124-108">De asemenea, instalarea poate să nu reușească dacă numărul total de instalări depășește numărul de licențe.</span><span class="sxs-lookup"><span data-stu-id="94124-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="94124-109">Pentru a vizualiza un raport de utilizare pentru licențele dvs. **Intune Mobile apps** , accesați pagina de \> **licențe** pentru aplicațiile mobile din Intune.</span><span class="sxs-lookup"><span data-stu-id="94124-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="94124-110">Pentru a afla cum să revendicați licențele în uz, consultați [acest articol.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="94124-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
