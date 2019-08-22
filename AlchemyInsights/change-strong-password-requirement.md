---
title: Schimbare parolă puternică cerinţă
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
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518771"
---
# <a name="change-strong-password-requirement"></a>Schimbare parolă puternică cerinţă

Microsoft necesită parole puternice în mod implicit. 

Folosind PowerShell, aveţi posibilitatea să dezactivaţi parolelor pentru utilizatorii specifice cu această comandă:<br>
*Set-MsolUser-UserPrincipalName <UserPrincipalName> -StrongPasswordRequired $false*

- [Mai multe informaţii despre politica de parola](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Cum să se conecteze la Office 365 cu PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Mai multe informaţii despre comenzile PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)