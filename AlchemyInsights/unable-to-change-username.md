---
title: Imposibil de modificat Numele utilizatorului
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440301"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="7cf5c-102">Imposibil de modificat Numele utilizatorului</span><span class="sxs-lookup"><span data-stu-id="7cf5c-102">Unable to change UserName</span></span>

<span data-ttu-id="7cf5c-103">În unele cazuri, modificările UPN (UserPrincipalName) nu sunt propagate în cloud.</span><span class="sxs-lookup"><span data-stu-id="7cf5c-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="7cf5c-104">Este posibil să primiți erori de validare în portalul Office 365 sau să nu reușiți să modificați numele de utilizator sau adresa de e-mail.</span><span class="sxs-lookup"><span data-stu-id="7cf5c-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="7cf5c-105">Pentru a rezolva această problemă, setați manual UserPrincipalName utilizând această comandă PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7cf5c-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="7cf5c-106">**Exemplu: Redenumirea unui utilizator**</span><span class="sxs-lookup"><span data-stu-id="7cf5c-106">**Example: Rename a user**</span></span>

<span data-ttu-id="7cf5c-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="7cf5c-107">PowerShellCopy</span></span>

<span data-ttu-id="7cf5c-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="7cf5c-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="7cf5c-109">Această comandă redenumește davidc@contoso.com în davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="7cf5c-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="7cf5c-110">Pentru mai multe informații, consultați [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="7cf5c-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>