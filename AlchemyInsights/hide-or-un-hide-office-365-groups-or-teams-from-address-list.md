---
title: Ascunderea sau ascunderea grupurilor Office 365 a echipelor din lista de adrese
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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088408"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Ascunderea sau ascunderea grupurilor Office 365 a echipelor din lista de adrese

Utilizați următoarea comandă EXO PowerShell pentru Office 365 ascunde sau a anula ascunderea grupurilor/echipelor Office 365 din listele de adrese (GAL) de clienți Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Utilizați următoarea comandă EXO PowerShell pentru a ascunde sau a anula ascunderea grupului/echipelor Office365 de la Exchange clienți (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Pentru instrucțiuni detaliate, [consultați Ascunderea Office 365 grupului din Gal și clienți Exchange clienți.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
