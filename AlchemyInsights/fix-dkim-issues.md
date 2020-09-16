---
title: Remedierea problemelor de configurare DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744962"
---
# <a name="fix-dkim-setup-issues"></a>Remedierea problemelor de configurare DKIM

Dacă întâmpinați probleme care permit DKIM pentru domeniul particularizat, utilizați următorii pași:

- Majoritatea problemelor de configurare DKIM sunt asociate înregistrărilor DNS incorecte. Verificați dacă înregistrarea CNAME DKIM (**nu** este o înregistrare txt) este formatat corect. Pentru mai multe informații, consultați acest [subiect](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- După ce creați sau actualizați înregistrările DNS DKIM la serviciul de găzduire DNS pentru domeniul dvs. (de obicei, Registratorul de domeniu), așteptați ca înregistrările DNS să se propage.

- Dacă nu puteți crea înregistrările DNS DKIM în centrul de administrare, puteți să înlocuiți \<CustomDomain\> cu domeniul particularizat (de exemplu, contoso.com) și să difuzați această comandă în [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
