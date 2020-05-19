---
title: Modificarea adresei de e-mail a unui grup Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283258"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Modificarea adresei de e-mail a unui grup Microsoft 365

Puteți modifica adresa de e-mail a unui grup Microsoft 365 utilizând centrul de administrare. Trebuie doar să selectați grupul și să selectați @edit adresa de e-mail.

De asemenea, aveți posibilitatea să utilizați urmând comanda EXO PowerShell pentru a modifica adresa SMTP principală a unui grup Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress Set-UnifiedGroup -PrimarySmtpAddress Set-UnifiedGroup -PrimarySmtpAddress Set-<new SMTP Address>

Exemplu:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
