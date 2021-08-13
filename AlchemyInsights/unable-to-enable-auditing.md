---
title: 2419-unable-to-enable-auditing
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007802"
---
# <a name="unable-to-enable-unified-auditing"></a>Nu se poate activa auditarea unificată

Când încercați să activați auditarea unificată pentru organizația dvs., este posibil să primiți o eroare similară cu următoarea:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Pentru a rezolva această problemă, urmați acești pași:

1. [Conectare la Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Rulați următorul cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Așteptați 60 de minute ca setarea anterioară să aibă efect.

4. Rulați următoarea comandă în Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Pentru informații suplimentare, consultați următoarele articole:

- [Conectare faceți Exchange Online PowerShell utilizând Multi-Factor Authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Activarea sau dezactivarea căutării în jurnalul de auditare](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
