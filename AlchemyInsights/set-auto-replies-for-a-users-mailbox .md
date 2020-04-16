---
title: Setarea răspunsurilor automate pentru cutia poștală a unui utilizator
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506529"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Setarea răspunsurilor automate pentru cutia poștală a unui utilizator

**Metoda 1**

1. Conectați-vă la portalul Office 365

2. Accesați **Utilizatori > Utilizatori activi** (sau **Grupuri > Cutii poștale partajate** dacă ați setat într-o cutie poștală partajată).

3. Selectați un utilizator care are o cutie poștală Microsoft Exchange.

4. În meniul mobil din dreapta, accesați **Setări de e-mail > Răspunsuri automate** (dacă este vorba de o cutie poștală partajată, faceți pur și simplu clic pe **Răspunsuri automate** din meniul mobil).

**Metoda 2**

1. Conectați-vă la portalul de administrare Office 365 utilizând acreditări de administrator.

2. Extindeți **Centre de administrare**, apoi faceți clic pe **Exchange**.

3. Faceți clic pe imaginea din colțul din dreapta sus, pe **Alt utilizator**, apoi selectați cutia poștală de utilizator pe care doriți să o modificați.

4. În partea stângă, selectați **Opțiuni**, faceți clic pe **Organizare e-mail**, apoi pe **Răspunsuri automate.**

**Metoda 3**

Rulați următorul cmdlet în Exchange Online PowerShell:

PowerShellCopy

    Set-MailboxAutoReplyConfiguration

Pentru mai multe informații despre acest cmdlet, consultați [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
