---
title: Instrucțiuni pentru ascunderea/dezascunderea grupului din lista de adrese
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768944"
---
# <a name="hide-office-365-group-from-address-list-gal"></a><span data-ttu-id="ace36-102">Ascundere grup 365 Office din lista de adrese (GAL)</span><span class="sxs-lookup"><span data-stu-id="ace36-102">Hide Office 365 group from address list (GAL)</span></span>

<span data-ttu-id="ace36-103">Pentru a ascunde un grup de Office 365 din listele de adrese (GAL) de clienți Exchange (cum ar fi Outlook sau OWA), utilizați următoarea comandă în Shell EXO:</span><span class="sxs-lookup"><span data-stu-id="ace36-103">To hide an Office 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="ace36-104">Pentru a ascunde grupul Office 365 de la a fi vizibile pentru clienții Exchange, utilizați următoarea comandă în Shell EXO:</span><span class="sxs-lookup"><span data-stu-id="ace36-104">To hide the Office 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

