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
# <a name="unable-to-change-username"></a>Imposibil de modificat Numele utilizatorului

În unele cazuri, modificările UPN (UserPrincipalName) nu sunt propagate în cloud. Este posibil să primiți erori de validare în portalul Office 365 sau să nu reușiți să modificați numele de utilizator sau adresa de e-mail. Pentru a rezolva această problemă, setați manual UserPrincipalName utilizând această comandă PowerShell.

**Exemplu: Redenumirea unui utilizator**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Această comandă redenumește davidc@contoso.com în davidchew@contoso.com.

Pentru mai multe informații, consultați [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).