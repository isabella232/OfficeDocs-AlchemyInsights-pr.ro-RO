---
title: Setarea ClientAccessServerEnabled la True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320368"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Setarea ClientAccessServerEnabled la True

Dacă nu puteți deschide un mesaj de e-mail criptat și în schimb vedeți o atașare **rpmsg,** efectuați pașii următori:

1. Conectare la Exchange Online PowerShell.

    **Notă:** Pentru a vă Exchange Online cu PowerShell, trebuie să vă conectați utilizând un cont de administrator global Exchange de administrator.

   a. Deschideți Windows PowerShell, apoi rulați următoarea comandă:`$UserCredential = Get-Credential`
   b. În caseta de **dialog Windows PowerShell de acreditări,** introduceți contul și parola de la locul de muncă sau de la școală, c. Faceți clic pe **OK**. 

2. Rulați următoarea comandă pentru a crea o nouă sesiune:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Rulați următoarea comandă:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Comanda `Get-IRMConfiguration` Rulare.

4. Verificați **setarea ClientAccessServerEnabled.** 

    a. Dacă **setarea ClientAccessServerEnabled** este setată **la False**, rulați următorul cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Sfat:** Închideți întotdeauna sesiunea PowerShell cu următoarea comandă: `Remove-PSSession $Session`

Pentru mai multe informații, [consultați Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

