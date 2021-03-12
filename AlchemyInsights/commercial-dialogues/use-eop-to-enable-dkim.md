---
title: Utilizarea Exchange Online PowerShell pentru a activa DKIM pentru un anumit domeniu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749728"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Utilizarea Exchange Online PowerShell pentru a activa DKIM pentru un anumit domeniu

Dacă nu puteți crea înregistrările DNS DKIM în centrul de administrare, încercați să utilizați Exchange Online PowerShell. 

Pentru a crea o înregistrare DNS DKIM utilizând Exchange Online PowerShell, efectuați pașii următori:

1. Deschideți Windows PowerShell ca administrator și rulați următoarele comenzi în secvența descrisă:

    un. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Dacă aveți probleme la conectarea la Exchange Online PowerShell, consultați [conectarea la Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. După ce sunteți conectat la Exchange Online PowerShell, derulează următoarea comandă:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. După ce comanda de mai sus a fost executată cu succes, rulați următoarea comandă pentru a rezilia sesiunea Exchange Online PowerShell:

    `Remove-PSSession $Session` 



