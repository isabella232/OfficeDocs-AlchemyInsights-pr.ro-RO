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
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070324"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Utilizarea Exchange Online PowerShell pentru a activa DKIM pentru un anumit domeniu

Dacă nu puteți crea înregistrăriLE DNS DKIM în centrul de administrare, încercați să utilizați Exchange Online PowerShell. 

Pentru a crea o înregistrare DNS DKIM utilizând Exchange Online PowerShell, efectuați pașii următori:

1. Deschideți Windows PowerShell ca administrator și rulați următoarele comenzi în secvența descrisă:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Dacă aveți probleme la conectarea la Exchange Online PowerShell, consultați [Conectare cu Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. După ce vă conectați la Exchange Online PowerShell, rulați următoarea comandă:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Odată ce comanda de mai sus a fost executată cu succes, rulați următoarea comandă pentru a Exchange Online sesiunea PowerShell:

    `Remove-PSSession $Session` 



