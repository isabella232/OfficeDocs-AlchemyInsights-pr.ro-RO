---
title: 932 actualizarea AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 0bbb847bb1381330065ebba6e109795908b06490
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/22/2019
ms.locfileid: "30778753"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="b530d-102">Upgrade azuriu AD conecta</span><span class="sxs-lookup"><span data-stu-id="b530d-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="b530d-103">În mod implicit, actualizarea automată este activată pentru Azure Connect AD, care ajută pentru a vă asigura că rulaţi cea mai recentă versiune.</span><span class="sxs-lookup"><span data-stu-id="b530d-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="b530d-104">Pentru a verifica setările de actualizare automată, utilizaţi cmdletul **Get-ADSyncAutoUpgrade** din PowerShell de AD Azure.</span><span class="sxs-lookup"><span data-stu-id="b530d-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="b530d-105">Cmdlet va returna una dintre următoarele valori:</span><span class="sxs-lookup"><span data-stu-id="b530d-105">The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="b530d-106">**Enabled**: actualizarea automată este activată.</span><span class="sxs-lookup"><span data-stu-id="b530d-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="b530d-107">**Cu handicap**: upgrade-ul automat este dezactivat.</span><span class="sxs-lookup"><span data-stu-id="b530d-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="b530d-108">**Suspendat**: sistemul nu mai este eligibil pentru a primi upgrade-uri automate.</span><span class="sxs-lookup"><span data-stu-id="b530d-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="b530d-109">Nu pot configura această valoare; Acesta este situat în sistemul de.</span><span class="sxs-lookup"><span data-stu-id="b530d-109">You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="b530d-110">Pentru informaţii suplimentare, consultaţi [actualizarea automată](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="b530d-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="b530d-111">Pentru a descărca cea mai recentă versiune de Azure AD Connect, du-te la [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="b530d-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

