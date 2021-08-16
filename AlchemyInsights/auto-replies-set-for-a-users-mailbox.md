---
title: Setarea răspunsurilor automate pentru o cutie poștală
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
- "9000761"
- "3514"
ms.openlocfilehash: 85b7e969032607216c948532dcdf83ba09022c7cdfaebce8671c6d2e8fef183d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046620"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Setarea răspunsurilor automate pentru cutia poștală a unui utilizator

**Metoda 1**

1. Conectați-vă la portalul Microsoft 365

2. Accesați **Utilizatori > Utilizatori activi** (sau **Grupuri > Cutii poștale partajate** dacă ați setat într-o cutie poștală partajată).

3. Selectați un utilizator care are o cutie poștală Microsoft Exchange.

4. În meniul mobil din dreapta, accesați **Setări de e-mail > Răspunsuri automate** (dacă este vorba de o cutie poștală partajată, faceți pur și simplu clic pe **Răspunsuri automate** din meniul mobil).

**Metoda 2**

1. Conectați-vă la portalul administrator Microsoft 365 utilizând acreditări de administrator.

2. Extindeți **Centre de administrare**, apoi faceți clic pe **Exchange**.

3. Faceți clic pe imaginea din colțul din dreapta sus, pe **Alt utilizator**, apoi selectați cutia poștală de utilizator pe care doriți să o modificați.

4. În partea stângă, selectați **Opțiuni**, faceți clic pe **Organizare e-mail**, apoi pe **Răspunsuri automate.**

**Metoda 3**

Rulați următorul cmdlet în Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Pentru mai multe informații despre acest cmdlet, consultați [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
