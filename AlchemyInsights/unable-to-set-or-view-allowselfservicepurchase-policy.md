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
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020204"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nu se poate seta sau vizualiza politica AllowServicePurchase

Atunci când încercați să setați sau să vizualizați politica AllowServicePurchase, primiți următorul mesaj de eroare:

*HandleError: Nu s-a reușit regăsirea politicii de produs cu PolicyId 'AllowServicePurchase', ErrorMessage - Conexiunea subiacentă a fost închisă: Eroare neașteptată la o trimitere.*

Acest lucru poate fi cauzat de o versiune mai veche de Transport Layer Security (TLS). Pentru a conecta serviciul MSCommerce, trebuie să utilizați TLS 1.2 sau o valoare ulterioară.  

Încercați următorii pași pentru a activa/a seta protocolul TLS la 1.2, a verifica și a reîncerca.
 1. În linia de comandă PowerShell (PS C: introduceți următoarea comandă pentru a seta protocolul \) TLS la versiunea 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Verificați protocoalele TLS utilizate, cu următoarea comandă:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Reîncercați comenzile Obțineți sau Actualizați după cum este necesar.

