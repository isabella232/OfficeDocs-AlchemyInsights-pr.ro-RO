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
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926257"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ascunderea Microsoft 365 grup din lista de adrese (GAL)

Pentru a ascunde un grup de Microsoft 365 din listele de adrese (GAL) de clienți Exchange (cum ar fi Outlook sau OWA), utilizați următoarea comandă în shell EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Pentru a ascunde Microsoft 365 grup de clienți potențiali este vizibil pentru Exchange, utilizați următoarea comandă în shell EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

