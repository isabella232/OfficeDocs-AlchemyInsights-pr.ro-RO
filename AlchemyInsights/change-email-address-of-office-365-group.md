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
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="c18dc-102">Modificarea adresei de e-mail a unui grup Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c18dc-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="c18dc-103">Puteți modifica adresa de e-mail a unui grup Microsoft 365 utilizând centrul de administrare.</span><span class="sxs-lookup"><span data-stu-id="c18dc-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="c18dc-104">Trebuie doar să selectați grupul și să selectați @edit adresa de e-mail.</span><span class="sxs-lookup"><span data-stu-id="c18dc-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="c18dc-105">De asemenea, aveți posibilitatea să utilizați urmând comanda EXO PowerShell pentru a modifica adresa SMTP principală a unui grup Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="c18dc-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="c18dc-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress Set-UnifiedGroup -PrimarySmtpAddress Set-UnifiedGroup -PrimarySmtpAddress Set-<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="c18dc-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="c18dc-107">Exemplu:</span><span class="sxs-lookup"><span data-stu-id="c18dc-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
