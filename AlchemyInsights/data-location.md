---
title: Locația datelor
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655294"
---
# <a name="data-location"></a><span data-ttu-id="81064-102">Locația datelor</span><span class="sxs-lookup"><span data-stu-id="81064-102">Data location</span></span>

<span data-ttu-id="81064-103">Puteți vizualiza locația entității găzduite în centrul de administrare sau conectându-vă la Exchange Online prin PowerShell.</span><span class="sxs-lookup"><span data-stu-id="81064-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="81064-104">**Centru de administrare:**</span><span class="sxs-lookup"><span data-stu-id="81064-104">**Admin center:**</span></span>
1. <span data-ttu-id="81064-105">Conectați-vă la centrul de [administrare](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="81064-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="81064-106">Selectaþi Profil**organizare** **setãri** > .</span><span class="sxs-lookup"><span data-stu-id="81064-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="81064-107">Sub **Locație date**, selectați Vizualizare **detalii**.</span><span class="sxs-lookup"><span data-stu-id="81064-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="81064-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="81064-108">**PowerShell:**</span></span>
1. <span data-ttu-id="81064-109">Conectați-vă la Exchange Online utilizând Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="81064-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="81064-110">Executați cmdletul [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) pentru a afișa o listă a proprietăților entității găzduite.</span><span class="sxs-lookup"><span data-stu-id="81064-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="81064-111">Uită-te la proprietatea OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="81064-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="81064-112">Când aveți locația de date pentru EXO și SPO, puteți determina locația de date pentru alte servicii pe care le puteți utiliza din [Locul în care se află datele dvs.](https://products.office.com/where-is-your-data-located)</span><span class="sxs-lookup"><span data-stu-id="81064-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>