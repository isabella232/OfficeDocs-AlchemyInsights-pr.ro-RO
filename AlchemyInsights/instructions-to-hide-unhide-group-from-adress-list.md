---
title: Instrucțiuni pentru ascunderea/reafișarea grupului din lista de adrese
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
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831890"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="c8fde-102">Ascunderea grupului Microsoft 365 din lista de adrese (GAL)</span><span class="sxs-lookup"><span data-stu-id="c8fde-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="c8fde-103">Pentru a ascunde un grup Microsoft 365 din listele de adrese (GAL) de clienți Exchange (cum ar fi Outlook sau OWA), utilizați următoarea comandă în shell EXO:</span><span class="sxs-lookup"><span data-stu-id="c8fde-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="c8fde-104">Pentru a ascunde grupul Microsoft 365 pentru a nu fi vizibil pentru clienții Exchange, utilizați următoarea comandă în exo shell:</span><span class="sxs-lookup"><span data-stu-id="c8fde-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

