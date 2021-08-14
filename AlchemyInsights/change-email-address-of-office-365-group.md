---
title: Modificarea adresei de e-mail a unui Microsoft 365 grup
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
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930741"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Modificarea adresei de e-mail a unui Microsoft 365 grup

Puteți modifica adresa de e-mail a unui Microsoft 365 grup utilizând centrul de administrare. Pur și simplu selectați grupul și selectați @editare adresă de e-mail.

De asemenea, puteți utiliza următoarele comenzi EXO PowerShell pentru a schimba adresa SMTP principală a unui Microsoft 365 grup:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Exemplu:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
