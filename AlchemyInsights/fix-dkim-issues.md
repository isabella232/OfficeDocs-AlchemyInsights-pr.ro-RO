---
title: Repara problemele de configurare DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765329"
---
# <a name="fix-dkim-setup-issues"></a>Repara problemele de configurare DKIM

Dacă vă confruntaţi cu probleme care să permită DKIM pentru domeniu personalizat, utilizaţi paşii următori:

- Cele mai multe probleme de configurare DKIM sunt legate de înregistrări DNS incorecte. Verificaţi dacă înregistrarea DKIM CNAME (**nu** o înregistrare TXT) este formatat corect. Pentru informaţii suplimentare, consultaţi acest [subiect](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- După ce creaţi sau actualizaţi înregistrări DKIM DNS la serviciul pentru domeniu (de obicei, Registratorul de domeniu) de găzduire DNS, aşteptaţi pentru înregistrările DNS pentru a propaga.

- Dacă nu puteţi crea DKIM DNS records în centrul de admin, aveţi posibilitatea să înlocuiţi \<CustomDomain\> cu domeniu personalizat (de exemplu, contoso.com) şi rulaţi această comandă în [PowerShell Online de schimb](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
