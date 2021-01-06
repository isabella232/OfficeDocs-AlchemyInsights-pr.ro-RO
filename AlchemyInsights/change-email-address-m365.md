---
title: Modificarea adresei de e-mail a unui grup Microsoft 365 sau Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756569"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Modificarea adresei de e-mail a unui grup Microsoft 365 sau Microsoft Teams

Puteți să modificați adresa de e-mail a unui grup Microsoft 365 sau al Microsoft Teams utilizând [centrul de administrare Microsoft 365](https://admin.microsoft.com/). Pur și simplu selectați grupul și selectați @editare adresă de e-mail.

De asemenea, puteți utiliza următoarea comandă EXO PowerShell pentru a modifica adresa SMTP principală a unui grup/Teams Microsoft 365:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exemplu:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
