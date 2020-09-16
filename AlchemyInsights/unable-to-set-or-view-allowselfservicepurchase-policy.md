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
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nu puteți seta sau vizualiza politica AllowSelfServicePurchase

Atunci când încercați să setați sau să vizualizați politica AllowSelfServicePurchase, primiți următorul mesaj de eroare:

*HandleError: nu s-a reușit regăsirea politicii de produs cu PolicyId ' AllowSelfServicePurchase ', ErrorMessage-conexiunea subiacentă a fost închisă: s-a produs o eroare neașteptată la trimitere.*

Acest lucru poate fi cauzat de o versiune mai veche de transport Layer Security (TLS). Pentru a conecta serviciul MSCommerce, trebuie să utilizați TLS 1,2 sau o versiune ulterioară.  

Încercați următorii pași pentru a activa/seta protocolul TLS la 1,2, verificați și încercați din nou.
 1. În linia de comandă PowerShell (PS C: \) Introduceți următoarea comandă pentru a seta protocolul TLS la versiunea 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Verificați dacă sunt utilizate protocoalele TLS, cu următoarea comandă:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Încercați din nou comenzile obțineți sau actualizați după cum este necesar.

