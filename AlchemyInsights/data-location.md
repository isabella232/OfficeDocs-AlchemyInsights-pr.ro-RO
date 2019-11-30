---
title: Locație de date
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
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627858"
---
# <a name="data-location"></a><span data-ttu-id="a9d23-102">Locație de date</span><span class="sxs-lookup"><span data-stu-id="a9d23-102">Data location</span></span>

<span data-ttu-id="a9d23-103">Puteți vizualiza locația entității găzduite Office 365 în centrul de administrare sau prin conectarea la Exchange Online prin PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a9d23-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="a9d23-104">**Centrul de administrare:**</span><span class="sxs-lookup"><span data-stu-id="a9d23-104">**Admin center:**</span></span>
1. <span data-ttu-id="a9d23-105">Conectați-vă la [Centrul de administrare](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="a9d23-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="a9d23-106">Selectați **Setări** > **profil organizație**.</span><span class="sxs-lookup"><span data-stu-id="a9d23-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="a9d23-107">Sub **locație de date**, selectați **Vizualizați detaliile**.</span><span class="sxs-lookup"><span data-stu-id="a9d23-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="a9d23-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="a9d23-108">**PowerShell:**</span></span>
1. <span data-ttu-id="a9d23-109">Conectați-vă la Exchange Online utilizând Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a9d23-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="a9d23-110">Executați cmdletul [Get-Organizalunit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) pentru a afișa o listă de proprietățile entității găzduite.</span><span class="sxs-lookup"><span data-stu-id="a9d23-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="a9d23-111">Uită-te la proprietatea OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="a9d23-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="a9d23-112">Când aveți locația de date pentru EXO și SPO, puteți determina locația de date pentru alte servicii pe care le puteți utiliza de [unde se află datele](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="a9d23-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>