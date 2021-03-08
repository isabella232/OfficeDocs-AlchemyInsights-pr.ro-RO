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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525964"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Setarea ClientAccessServerEnabled la True

Dacă nu puteți deschide un mesaj de e-mail criptat și vedeți în schimb o atașare **rpmsg** , efectuați pașii următori:

1. Conectați-vă la Exchange Online PowerShell.

> [!NOTE]
> Pentru a vă conecta la Exchange Online PowerShell, trebuie să vă conectați utilizând un cont de administrator global sau Exchange.

   un. Deschideți Windows PowerShell, apoi rulează următoarea comandă: `$UserCredential = Get-Credential`
b. În caseta de dialog **solicitare de acreditare Windows PowerShell** , introduceți contul de la locul de muncă sau de la școală și parola, c. Faceți clic pe **OK**. 

2. Rulează următoarea comandă pentru a crea o sesiune nouă:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    un. Rulați următoarea comandă:
    
    `Import-PSSession $Session -DisableNameChecking`

3. `Get-IRMConfiguration`Comanda rulare.

4. Verificați setarea **ClientAccessServerEnabled** . 

    un. Dacă setarea **ClientAccessServerEnabled** este setată la **false**, rulează următorul cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Închideți întotdeauna sesiunea PowerShell cu următoarea comandă: `Remove-PSSession $Session`

Pentru mai multe informații, consultați [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

