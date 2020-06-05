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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580669"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Modificarea adresei de e-mail a unui grup Microsoft 365

Puteți modifica adresa de e-mail a unui grup Microsoft 365 utilizând centrul de administrare. Trebuie doar să selectați grupul și să selectați @edit adresa de e-mail.

De asemenea, aveți posibilitatea să utilizați urmând comanda EXO PowerShell pentru a modifica adresa SMTP principală a unui grup Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress Set-UnifiedGroup -PrimarySmtpAddress Set-UnifiedGroup -PrimarySmtpAddress Set-<new SMTP Address>

Exemplu:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
