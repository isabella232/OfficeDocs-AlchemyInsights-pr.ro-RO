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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819092"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="c8304-102">Modificarea adresei de e-mail a unui grup Microsoft 365 sau Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c8304-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="c8304-103">Puteți să modificați adresa de e-mail a unui grup Microsoft 365 sau al Microsoft Teams utilizând [centrul de administrare Microsoft 365](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="c8304-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="c8304-104">Pur și simplu selectați grupul și selectați @editare adresă de e-mail.</span><span class="sxs-lookup"><span data-stu-id="c8304-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="c8304-105">De asemenea, puteți utiliza următoarea comandă EXO PowerShell pentru a modifica adresa SMTP principală a unui grup/Teams Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="c8304-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="c8304-106">Exemplu:</span><span class="sxs-lookup"><span data-stu-id="c8304-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
