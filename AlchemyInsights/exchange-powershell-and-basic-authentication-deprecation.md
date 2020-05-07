---
title: Exchange PowerShell și perimarea autentificării de bază
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015701"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell și perimarea autentificării de bază

Pentru cele mai recente informații despre cum să vă conectați la Exchange Online PowerShell fără să utilizați autentificarea de bază, [accesați aici](https://aka.ms/psbasicauth).

Rețineți că autentificarea de bază trebuie să fie în continuare activată pe computerul client.
Noul modul PowerShell V2 utilizează Autentificarea modernă pentru a stabili o conexiune în vederea activării tuturor cmdleturilor V2 bazate pe REST. Pe lângă cmdleturile V2, aveți permisiunea să accesați cmdleturile mai vechi PowerShell de la distanță (RPS) care necesită stabilirea unei sesiuni PowerShell la distanță. Stabilirea unei sesiuni RPS pe computerul Windows necesită activarea WinRM BasicAuth pe computerul client, chiar dacă modulul utilizează mecanismul de Autentificare modernă pentru a se autentifica la serviciu. Canalul WinRM Basic Auth este utilizat pentru transportul simbolurilor Autentificării moderne. Dacă WinRM Basic Auth este dezactivată pe computerul client, noile cmdleturi V2 vor continua să funcționeze (dar cmdleturile RPS mai vechi nu vor mai funcționa).
