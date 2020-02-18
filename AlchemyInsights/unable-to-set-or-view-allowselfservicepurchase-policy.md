---
title: Imposibil de setat sau vizualizat politica AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091750"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="d24e2-102">Imposibil de setat sau vizualizat politica AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="d24e2-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="d24e2-103">Când încercați să setați sau vizualizați politica AllowSelfServicePurchase, primiți următorul mesaj de eroare:</span><span class="sxs-lookup"><span data-stu-id="d24e2-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="d24e2-104">*HandleError: Nu a reușit să regăsiți politica de produs cu PolicyId 'AllowSelfServicePurchase', ErrorMessage - conexiunea subiacentă a fost închisă: a apărut o eroare neașteptată pe o trimitere.*</span><span class="sxs-lookup"><span data-stu-id="d24e2-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="d24e2-105">Acest lucru se poate datora unei versiuni mai vechi de Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="d24e2-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="d24e2-106">Pentru a conecta serviciul MSCommerce, trebuie să utilizați TLS 1.2 sau o versiune ulterioară.</span><span class="sxs-lookup"><span data-stu-id="d24e2-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="d24e2-107">Încercați următorii pași pentru a activa/seta protocolul TLS la 1.2, verificați și încercați din nou.</span><span class="sxs-lookup"><span data-stu-id="d24e2-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="d24e2-108">La promptul de comandă PowerShell (PS C:\) introduceți următoarea comandă pentru a seta protocolul TLS la versiunea 1.2:</span><span class="sxs-lookup"><span data-stu-id="d24e2-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="d24e2-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span><span class="sxs-lookup"><span data-stu-id="d24e2-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="d24e2-110">Verificați protocoalele TLS în uz, cu următoarea comandă:</span><span class="sxs-lookup"><span data-stu-id="d24e2-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="d24e2-111">\[Net.ServicePointManager]::Protocol de securitate</span><span class="sxs-lookup"><span data-stu-id="d24e2-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="d24e2-112">Încercați din nou comenzile Obțineți sau actualizați după este necesar.</span><span class="sxs-lookup"><span data-stu-id="d24e2-112">Retry the Get or Update commands as needed.</span></span>

