---
title: Modificarea adresei de e-mail a grupului Microsoft 365
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
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/10/2020
ms.locfileid: "48461949"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Modificarea adresei de e-mail a unui grup Microsoft 365

Puteți să modificați adresa de e-mail a unui grup Microsoft 365 utilizând Centrul de administrare. Pur și simplu selectați grupul și selectați @edit adresă de e-mail.

De asemenea, puteți să utilizați următoarea comandă EXO PowerShell pentru a modifica adresa SMTP principală a unui grup Microsoft 365:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exemplu

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
