---
title: Exchange PowerShell și perimarea autentificării de bază
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813484"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell și perimarea autentificării de bază

Pentru cele mai recente informații despre cum să vă conectați la Exchange Online PowerShell fără să utilizați autentificarea de bază, [accesați aici](https://aka.ms/exops-docs). Modulul PowerShell V2 nu utilizează autentificarea de bază.

Rețineți că autentificarea de bază trebuie să fie în continuare activată pe computerul client.
Noul modul PowerShell V2 utilizează Autentificarea modernă pentru a stabili o conexiune în vederea activării tuturor cmdleturilor V2 bazate pe REST. Pe lângă cmdleturile V2, aveți permisiunea să accesați cmdleturile mai vechi PowerShell de la distanță (RPS) care necesită stabilirea unei sesiuni PowerShell la distanță. Stabilirea unei sesiuni RPS pe computerul Windows necesită activarea WinRM BasicAuth pe computerul client, chiar dacă modulul utilizează mecanismul de Autentificare modernă pentru a se autentifica la serviciu. Canalul WinRM Basic Auth este utilizat pentru transportul simbolurilor Autentificării moderne. Dacă WinRM Basic Auth este dezactivată pe computerul client, noile cmdleturi V2 vor continua să funcționeze (dar cmdleturile RPS mai vechi nu vor mai funcționa).
