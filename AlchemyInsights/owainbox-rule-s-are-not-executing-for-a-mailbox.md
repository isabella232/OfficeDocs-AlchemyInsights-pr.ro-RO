---
title: 1332 OWA - Reguli Inbox nu se execută pentru o cutie poștală
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576572"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>O regulă Inbox nu funcționează conform așteptărilor

Verificați următoarele setări în Outlook pe web:

- Un mesaj poate fi redirecționat, redirecționat sau răspuns automat pe baza regulilor Inbox o singură dată. O regulă de redirecționare (o regulă Inbox sau o regulă de flux de corespondență, cunoscută și ca regulă de transport) poate adăuga maximum zece destinatari de redirecționare la un mesaj. Pentru mai multe informații, consultați [Limitele de regulă Jurnal, Transport și Inbox](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Regulile inbox nu funcționează pe cutia poștală de jurnalizare alternativ. Pentru mai multe informații despre cutia poștală alternativă de jurnalizare, consultați [Căsuța poștală alternativă de jurnalizare](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Pentru a remedia aceste probleme, consultați [KB 2829319](https://support.microsoft.com/kb/2829319).

Dacă problemele anterioare nu se aplică, executați raportul de diagnosticare a regulii Inbox înainte de a escalada problema la Microsoft Support:

1. Deschideți cutia poștală în Outlook pe web și faceți clic pe <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Setări > Setări**  >  **Vezi toate setările**  >  Outlook **E-mail**  >  **Reguli**.

2. În partea de jos a paginii, faceți clic pe **Dacă regulile nu funcționează, faceți clic aici pentru a genera un raport de diagnosticare**.
