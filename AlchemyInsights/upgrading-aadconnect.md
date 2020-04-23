---
title: 932 Actualizarea AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766505"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="94c96-102">Upgrade Azure AD Conectați</span><span class="sxs-lookup"><span data-stu-id="94c96-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="94c96-103">În mod implicit, upgrade-ul automat este activat pentru Azure AD Connect, ceea ce vă ajută să vă asigurați că executați cea mai recentă versiune.</span><span class="sxs-lookup"><span data-stu-id="94c96-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="94c96-104">Pentru a verifica setările de upgrade automat, utilizați cmdletul **Get-ADSyncAutoUpgrade** în Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="94c96-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="94c96-105">Cmdletul va returna una dintre următoarele valori:</span><span class="sxs-lookup"><span data-stu-id="94c96-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="94c96-106">**Activat:** Este activată upgrade-ul automat.</span><span class="sxs-lookup"><span data-stu-id="94c96-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="94c96-107">**Dezactivat:** Upgrade-ul automat este dezactivat.</span><span class="sxs-lookup"><span data-stu-id="94c96-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="94c96-108">**Suspendat:** Sistemul nu mai este eligibil pentru a primi upgrade-uri automate.</span><span class="sxs-lookup"><span data-stu-id="94c96-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="94c96-109">Imposibil de configurat această valoare; Este setat de sistem.</span><span class="sxs-lookup"><span data-stu-id="94c96-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="94c96-110">Pentru mai multe informații, consultați [Upgrade automat](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="94c96-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="94c96-111">Pentru a descărca cea mai recentă versiune [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)de Azure AD Connect, accesați .</span><span class="sxs-lookup"><span data-stu-id="94c96-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
