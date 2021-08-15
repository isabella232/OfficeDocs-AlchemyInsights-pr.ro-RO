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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994877"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Setarea ClientAccessServerEnabled la True

Dacă nu puteți deschide un mesaj de e-mail criptat și în schimb vedeți o atașare **rpmsg,** efectuați pașii următori:

1. Conectare la Exchange Online PowerShell.

> [!NOTE]
> Pentru a vă conecta Exchange Online PowerShell, trebuie să vă conectați utilizând un administrator global sau un Exchange de administrator.

   a. Deschideți Windows PowerShell, apoi rulați următoarea comandă:`$UserCredential = Get-Credential`
b. În caseta de **dialog Windows PowerShell de acreditări,** introduceți contul de la locul de muncă sau de la școală și parola, c. Faceți clic pe **OK**. 

2. Rulați următoarea comandă pentru a crea o nouă sesiune:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Rulați următoarea comandă:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Comanda `Get-IRMConfiguration` Rulare.

4. Verificați **setarea ClientAccessServerEnabled.** 

    a. Dacă **setarea ClientAccessServerEnabled** este setată **la False**, rulați următorul cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Închideți întotdeauna sesiunea PowerShell cu următoarea comandă: `Remove-PSSession $Session`

Pentru mai multe informații, [consultați Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

