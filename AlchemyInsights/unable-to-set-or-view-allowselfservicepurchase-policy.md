---
title: Nu se poate seta sau vizualiza politica AllowServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826103"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="9121d-102">Nu se poate seta sau vizualiza politica AllowServicePurchase</span><span class="sxs-lookup"><span data-stu-id="9121d-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="9121d-103">Atunci când încercați să setați sau să vizualizați politica AllowServicePurchase, primiți următorul mesaj de eroare:</span><span class="sxs-lookup"><span data-stu-id="9121d-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="9121d-104">*HandleError: Nu s-a reușit regăsirea politicii de produs cu PolicyId 'AllowServicePurchase', ErrorMessage - Conexiunea subiacentă a fost închisă: Eroare neașteptată la o trimitere.*</span><span class="sxs-lookup"><span data-stu-id="9121d-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="9121d-105">Acest lucru poate fi cauzat de o versiune mai veche de Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="9121d-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="9121d-106">Pentru a conecta serviciul MSCommerce, trebuie să utilizați TLS 1.2 sau o valoare ulterioară.</span><span class="sxs-lookup"><span data-stu-id="9121d-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="9121d-107">Încercați următorii pași pentru a activa/a seta protocolul TLS la 1.2, a verifica și a reîncerca.</span><span class="sxs-lookup"><span data-stu-id="9121d-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="9121d-108">În linia de comandă PowerShell (PS C: introduceți următoarea comandă pentru a seta protocolul \) TLS la versiunea 1.2:</span><span class="sxs-lookup"><span data-stu-id="9121d-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="9121d-109">Verificați protocoalele TLS utilizate, cu următoarea comandă:</span><span class="sxs-lookup"><span data-stu-id="9121d-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="9121d-110">Reîncercați comenzile Obțineți sau Actualizați după cum este necesar.</span><span class="sxs-lookup"><span data-stu-id="9121d-110">Retry the Get or Update commands as needed.</span></span>

