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
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8038d5ef768d6ee228db7d038ad71d926f4047f3
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29937956"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="9ca80-102">Upgrade azuriu AD conecta</span><span class="sxs-lookup"><span data-stu-id="9ca80-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="9ca80-p101">În mod implicit, actualizarea automată este activată pentru Azure Connect AD, care ajută pentru a vă asigura că rulaţi cea mai recentă versiune. Pentru a verifica setările de actualizare automată, utilizaţi cmdletul **Get-ADSyncAutoUpgrade** din PowerShell de AD Azure. Cmdlet va returna una dintre următoarele valori:</span><span class="sxs-lookup"><span data-stu-id="9ca80-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="9ca80-106">**Enabled**: actualizarea automată este activată.</span><span class="sxs-lookup"><span data-stu-id="9ca80-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="9ca80-107">**Cu handicap**: upgrade-ul automat este dezactivat.</span><span class="sxs-lookup"><span data-stu-id="9ca80-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="9ca80-p102">**Suspendat**: sistemul nu mai este eligibil pentru a primi upgrade-uri automate. Nu pot configura această valoare; Acesta este situat în sistemul de.</span><span class="sxs-lookup"><span data-stu-id="9ca80-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="9ca80-110">Pentru informaţii suplimentare, consultaţi [actualizarea automată](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="9ca80-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="9ca80-111">Pentru a descărca cea mai recentă versiune de Azure AD Connect, du-te la [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="9ca80-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

