---
title: 2419-imposibil de-la-enable-audit
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065689"
---
# <a name="unable-to-enable-unified-auditing"></a>Imposibilitatea de a permite unificate de audit

Atunci când încercaţi să activaţi auditarea unificat pentru organizaţia Office 365, poate apărea o eroare similar cu următorul text:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Pentru a rezolva această problemă, urmaţi aceşti paşi:

1. [Connect pentru a face schimb de Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Executaţi următoarele cmdlet-ului:

   ```
   Enable-OrganizationCustomization
   ```

3. Aşteptaţi pentru 60 de minute pentru setarea anterioară să aibă efect.

4. Executaţi comanda următoare în Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Pentru informaţii suplimentare, consultaţi următoarele articole:

- [Conecta la Exchange Online PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Office 365 audit jurnal caută de activarea sau dezactivarea](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
