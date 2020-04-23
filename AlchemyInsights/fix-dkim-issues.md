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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717574"
---
# <a name="fix-dkim-setup-issues"></a>Remedierea problemelor de instalare DKIM

Dacă întâmpinați probleme care permit DKIM pentru domeniul particularizat, utilizați următorii pași:

- Cele mai multe probleme de instalare DKIM sunt legate de înregistrări DNS incorecte. Verificați înregistrarea DKIM CNAME **(nu** o înregistrare TXT) este formatat corect. Pentru mai multe informații, consultați acest [subiect](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- După ce creați sau actualizați înregistrările DKIM DNS la serviciul de găzduire DNS pentru domeniul dvs., așteptați ca înregistrările DNS să se propage.

- Dacă nu se pot crea înregistrările DKIM DNS în \<centrul\> de administrare, aveți posibilitatea să înlocuiți CustomDomain cu domeniul `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`particularizat (de exemplu, contoso.com) și să executați această comandă în Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): .
