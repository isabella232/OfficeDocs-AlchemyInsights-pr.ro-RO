---
title: 2419-imposibil de activat-audit
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767611"
---
# <a name="unable-to-enable-unified-auditing"></a>Nu se poate activa auditarea unificată

Atunci când încercați să activați auditarea unificată pentru organizația dvs., este posibil să primiți o eroare similară cu următoarea:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Pentru a rezolva această problemă, urmați acești pași:

1. [Conectați-vă la Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Rulează următorul cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Așteptați 60 de minute pentru ca setarea anterioară să aibă efect.

4. Rulează următoarea comandă în Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Pentru informații suplimentare, consultați următoarele articole:

- [Conectarea la Exchange Online PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Activarea sau dezactivarea căutării în Jurnalul de auditare](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
