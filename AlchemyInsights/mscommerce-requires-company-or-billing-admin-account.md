---
title: Conectarea la modulul MSCommerce
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 80735a03eef6ef9f7b791c43019678ea01f83c00
ms.sourcegitcommit: 9db3be25d088b8d4b2d476aeace79e653ca0a421
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/17/2020
ms.locfileid: "42093616"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="1118f-102">MSCommerce necesită un cont de companie sau de administrator de facturare</span><span class="sxs-lookup"><span data-stu-id="1118f-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="1118f-103">Modulul MSCommerce necesită un cont cu privilegii de administrator de companie sau facturare.</span><span class="sxs-lookup"><span data-stu-id="1118f-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="1118f-104">Dacă primiți următoarea eroare, va trebui să vă reconectați cu un alt cont.</span><span class="sxs-lookup"><span data-stu-id="1118f-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

    ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - 
    At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5
    +     HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...
    +     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
        + CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException
        + FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError

<span data-ttu-id="1118f-105">În cazul în care contul nu are privilegii de Administrator de companie sau de facturare, contactați administratorul IT.</span><span class="sxs-lookup"><span data-stu-id="1118f-105">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
