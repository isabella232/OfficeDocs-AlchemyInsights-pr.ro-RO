---
title: Ascunderea sau ascunderea grupurilor sau echipelor Office 365 din lista de adrese
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811468"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Ascunderea sau ascunderea grupurilor sau echipelor Office 365 din lista de adrese

Utilizați următoarea comandă EXO PowerShell pentru a ascunde sau a ascunde grupul/echipele Office 365 din listele de adrese (GAL) de clienți Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Utilizați următoarea comandă EXO PowerShell pentru a ascunde sau a ascunde grupul/echipele Office365 de la clienții Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Pentru instrucțiuni detaliate, [consultați Ascunderea grupurilor Office 365 din clienți GAL și Exchange.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
