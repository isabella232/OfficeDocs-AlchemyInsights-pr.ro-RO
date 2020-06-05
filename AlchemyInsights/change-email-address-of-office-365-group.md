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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="a3476-102">Modificarea adresei de e-mail a unui grup Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a3476-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="a3476-103">Puteți modifica adresa de e-mail a unui grup Microsoft 365 utilizând centrul de administrare.</span><span class="sxs-lookup"><span data-stu-id="a3476-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="a3476-104">Trebuie doar să selectați grupul și să selectați @edit adresa de e-mail.</span><span class="sxs-lookup"><span data-stu-id="a3476-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="a3476-105">De asemenea, aveți posibilitatea să utilizați urmând comanda EXO PowerShell pentru a modifica adresa SMTP principală a unui grup Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="a3476-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="a3476-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress Set-UnifiedGroup -PrimarySmtpAddress Set-UnifiedGroup -PrimarySmtpAddress Set-<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="a3476-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="a3476-107">Exemplu:</span><span class="sxs-lookup"><span data-stu-id="a3476-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
