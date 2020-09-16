---
title: Nu puteți seta sau vizualiza politica AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735211"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="72ef7-102">Nu puteți seta sau vizualiza politica AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="72ef7-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="72ef7-103">Atunci când încercați să setați sau să vizualizați politica AllowSelfServicePurchase, primiți următorul mesaj de eroare:</span><span class="sxs-lookup"><span data-stu-id="72ef7-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="72ef7-104">*HandleError: nu s-a reușit regăsirea politicii de produs cu PolicyId ' AllowSelfServicePurchase ', ErrorMessage-conexiunea subiacentă a fost închisă: s-a produs o eroare neașteptată la trimitere.*</span><span class="sxs-lookup"><span data-stu-id="72ef7-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="72ef7-105">Acest lucru poate fi cauzat de o versiune mai veche de transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="72ef7-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="72ef7-106">Pentru a conecta serviciul MSCommerce, trebuie să utilizați TLS 1,2 sau o versiune ulterioară.</span><span class="sxs-lookup"><span data-stu-id="72ef7-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="72ef7-107">Încercați următorii pași pentru a activa/seta protocolul TLS la 1,2, verificați și încercați din nou.</span><span class="sxs-lookup"><span data-stu-id="72ef7-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="72ef7-108">În linia de comandă PowerShell (PS C: \) Introduceți următoarea comandă pentru a seta protocolul TLS la versiunea 1,2:</span><span class="sxs-lookup"><span data-stu-id="72ef7-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="72ef7-109">Verificați dacă sunt utilizate protocoalele TLS, cu următoarea comandă:</span><span class="sxs-lookup"><span data-stu-id="72ef7-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="72ef7-110">Încercați din nou comenzile obțineți sau actualizați după cum este necesar.</span><span class="sxs-lookup"><span data-stu-id="72ef7-110">Retry the Get or Update commands as needed.</span></span>

