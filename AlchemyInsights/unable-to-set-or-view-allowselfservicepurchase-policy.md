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
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Imposibil de setat sau vizualizat politica AllowSelfServicePurchase

Când încercați să setați sau vizualizați politica AllowSelfServicePurchase, primiți următorul mesaj de eroare:

*HandleError: Nu a reușit să regăsiți politica de produs cu PolicyId 'AllowSelfServicePurchase', ErrorMessage - conexiunea subiacentă a fost închisă: a apărut o eroare neașteptată pe o trimitere.*

Acest lucru se poate datora unei versiuni mai vechi de Transport Layer Security (TLS). Pentru a conecta serviciul MSCommerce, trebuie să utilizați TLS 1.2 sau o versiune ulterioară.  

Încercați următorii pași pentru a activa/seta protocolul TLS la 1.2, verificați și încercați din nou.
 1. La promptul de comandă PowerShell (PS C:\) introduceți următoarea comandă pentru a seta protocolul TLS la versiunea 1.2:

    \[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12

2. Verificați protocoalele TLS în uz, cu următoarea comandă:

    \[Net.ServicePointManager]::Protocol de securitate 

3. Încercați din nou comenzile Obțineți sau actualizați după este necesar.

