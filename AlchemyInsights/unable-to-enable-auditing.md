---
title: 2419-incapabil-la-enable-auditare
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510440"
---
# <a name="unable-to-enable-unified-auditing"></a>Imposibil de activat auditarea unificată

Când încercați să activați auditarea unificată pentru organizația dvs., este posibil să primiți o eroare similară cu următoarea:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Pentru a rezolva această problemă, urmați acești pași:

1. [Conectare la Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Executați cmdletul următoarele:

   ```
   Enable-OrganizationCustomization
   ```

3. Așteptați 60 de minute pentru ca setarea anterioară să aibă efect.

4. Executați următoarea comandă în Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Pentru informații suplimentare, consultați următoarele articole:

- [Conectarea la Exchange Online PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Activarea sau dezactivarea căutării în jurnalul de audit](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
