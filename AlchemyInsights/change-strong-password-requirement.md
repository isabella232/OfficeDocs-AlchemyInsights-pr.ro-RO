---
title: Modificați cerința puternică de parolă
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070696"
---
# <a name="change-strong-password-requirement"></a>Modificați cerința puternică de parolă

Microsoft necesită parole puternice în mod implicit.

Cu ajutorul PowerShell, puteți dezactiva parole puternice pentru utilizatori cu aceste comenzi:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Pentru a dezactiva parolele puternice pentru toți utilizatorii, utilizați:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Mai multe informații despre politica pentru parole](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Cum să vă conectați la Microsoft 365 cu PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Mai multe informații despre comenzile MsolUser PowerShell](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
