---
title: Modificarea cerinței pentru parolă puternică
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: d888f4a208ccbc6f54469f5e1eb88f9f4197e5c9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47681884"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="698b1-102">Modificarea cerinței pentru parolă puternică</span><span class="sxs-lookup"><span data-stu-id="698b1-102">Change strong password requirement</span></span>

<span data-ttu-id="698b1-103">Microsoft necesită parole puternice în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="698b1-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="698b1-104">Utilizând PowerShell, puteți dezactiva parole puternice pentru anumiți utilizatori cu această comandă:</span><span class="sxs-lookup"><span data-stu-id="698b1-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="698b1-105">*Set-MsolUser-UserPrincipalName <UserPrincipalName> -StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="698b1-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="698b1-106">Mai multe informații despre politica prin parolă</span><span class="sxs-lookup"><span data-stu-id="698b1-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="698b1-107">Cum să vă conectați la Microsoft 365 cu PowerShell</span><span class="sxs-lookup"><span data-stu-id="698b1-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="698b1-108">Mai multe informații despre comenzile MsolUser PowerShell</span><span class="sxs-lookup"><span data-stu-id="698b1-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
