---
title: Remedierea problemelor de instalare DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506786"
---
# <a name="fix-dkim-setup-issues"></a>Remedierea problemelor de instalare DKIM

Dacă întâmpinați probleme care permit DKIM pentru domeniul particularizat, utilizați următorii pași:

- Cele mai multe probleme de instalare DKIM sunt legate de înregistrări DNS incorecte. Verificați înregistrarea DKIM CNAME **(nu** o înregistrare TXT) este formatat corect. Pentru mai multe informații, consultați acest [subiect](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- După ce creați sau actualizați înregistrările DKIM DNS la serviciul de găzduire DNS pentru domeniul dvs., așteptați ca înregistrările DNS să se propage.

- Dacă nu se pot crea înregistrările DKIM DNS în centrul de administrare, aveți posibilitatea să \<CustomDomain\> înlocuiți cu domeniul particularizat (de exemplu, contoso.com) și să executați această comandă în [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
