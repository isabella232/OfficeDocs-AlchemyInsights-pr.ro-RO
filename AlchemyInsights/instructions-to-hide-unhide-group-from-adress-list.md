---
title: Instrucțiuni pentru ascunderea/reafișarea grupului din lista de adrese
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
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580021"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ascundere grup Microsoft 365 din lista de adrese (GAL)

Pentru a ascunde un grup Microsoft 365 din listele de adrese (GAL) de clienți Exchange (cum ar fi Outlook sau OWA), utilizați următoarea comandă în shell EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Pentru a ascunde grupul Microsoft 365 de a fi vizibile pentru clienții Exchange, utilizați următoarea comandă în shell EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

