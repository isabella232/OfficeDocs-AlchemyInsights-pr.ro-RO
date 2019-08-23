---
title: 1332 OWA - Inbox rule(s) sunt nu executa pentru o cutie poştală
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 901237d4dc7b99695097142c61a4bfef7c09750d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36555785"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Regulă Inbox nu funcţionează conform aşteptărilor

Verificaţi următoarele setări în Outlook pe web:

- Un mesaj poate fi redirecţionat, altui tip de conþinut, sau a răspuns la automat bazat pe reguli Inbox numai o singură dată. O regulă de redirecţionare (o regulă Inbox sau mail fluxul de regulă, de asemenea, cunoscut ca o regulă de transport) puteţi adăuga maximum zece expediere destinatari la un mesaj. Pentru informaţii suplimentare, consultaţi [jurnal, Transport, şi Inbox limitele de regula](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Regulile pentru Inbox nu funcţionează pe cutia poştală de jurnalizare alternativ. Pentru mai multe informaţii despre cutia poştală de jurnalizare alternativă, a se vedea [poştală de jurnalizare alternativ](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Pentru a rezolva aceste probleme, a se vedea [KB 2829319](https://support.microsoft.com/kb/2829319).

În cazul în care problemele anterioare nu se aplică, executaţi raportul regulă Inbox de diagnosticare înainte să escaladeze emiterii către Microsoft Support:

1. Deschide cutia poştală în Outlook pe web, şi faceţi clic pe <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Setări** > **Vezi toate setările de Outlook** > **Mail** > **reguli**.

2. În partea de jos a paginii, faceţi clic pe **dacă regulile tale nu sunt de lucru faceţi clic aici pentru a genera un raport de diagnostic**.
