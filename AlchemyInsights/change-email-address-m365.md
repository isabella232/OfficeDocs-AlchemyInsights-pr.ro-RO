---
title: Modificarea adresei de e-mail a unui grup Microsoft 365 sau Microsoft Teams
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995634"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Modificarea adresei de e-mail a unui grup Microsoft 365 sau Microsoft Teams

Puteți să modificați adresa de e-mail a unui grup Microsoft 365 sau al Microsoft Teams utilizând [centrul de administrare Microsoft 365](https://admin.microsoft.com/). Pur și simplu selectați grupul și selectați @editare adresă de e-mail.

De asemenea, puteți utiliza următoarea comandă EXO PowerShell pentru a modifica adresa SMTP principală a unui grup/Teams Microsoft 365:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exemplu:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
