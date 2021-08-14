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
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945943"
---
# <a name="fix-dkim-setup-issues"></a>Remedierea problemelor de configurare DKIM

Dacă vă experimentați probleme la activarea DKIM pentru domeniul particularizat, urmați acești pași:

- Majoritatea problemelor de configurare DKIM sunt legate de înregistrări DNS incorecte. Verificați dacă înregistrarea DKIM CNAME **(nu** o înregistrare TXT) este formatată corect. Pentru mai multe informații, consultați acest [subiect.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- După ce creați sau actualizați înregistrările DNS DKIM la serviciul de găzduire DNS pentru domeniul dvs. (de obicei, registratorul de domeniu), așteptați propagarea înregistrărilor DNS.

- Dacă nu puteți crea înregistrările DNS DKIM în centrul de administrare, puteți să înlocuiți cu domeniul particularizat (de exemplu, contoso.com) și să rulați această comandă \<CustomDomain\> [în Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
