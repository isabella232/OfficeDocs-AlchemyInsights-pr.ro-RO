---
title: Modificare cerință parolă puternică
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286290"
---
# <a name="change-strong-password-requirement"></a>Modificarea cerinței de parolă puternică

Microsoft necesită parole puternice în mod implicit. 

Folosind PowerShell, poți dezactiva parolele puternice pentru anumiți utilizatori cu această comandă:<br>
*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired $false*

- [Mai multe informații despre politica privind parolele](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [să vă conectați la Office 365 cu PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Mai multe informații despre comenzile PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [Setarea parolei unui utilizator individual să nu expire niciodată](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
