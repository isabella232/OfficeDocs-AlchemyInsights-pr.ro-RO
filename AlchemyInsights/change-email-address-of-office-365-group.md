---
title: Modificarea adresei de e-mail a unui grup Microsoft 365
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
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819056"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Modificarea adresei de e-mail a unui grup Microsoft 365

Puteți modifica adresa de e-mail a unui grup Microsoft 365 utilizând centrul de administrare. Pur și simplu selectați grupul și selectați @editare adresă de e-mail.

De asemenea, puteți utiliza urmând comanda EXO PowerShell pentru a schimba adresa SMTP principală a unui grup Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Exemplu:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
