---
title: Setarea răspunsurilor automate pentru o cutie poștală
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
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788894"
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
