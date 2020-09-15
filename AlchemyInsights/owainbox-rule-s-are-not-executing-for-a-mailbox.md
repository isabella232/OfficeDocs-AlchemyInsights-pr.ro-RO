---
title: 1332 OWA-regulile pentru Inbox nu se execută pentru o cutie poștală
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721603"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>O regulă de Inbox nu funcționează așa cum vă așteptați

Verificați următoarele setări în Outlook pe web:

- Un mesaj poate fi Redirecționat, Redirecționat sau răspuns la automat, în funcție de regulile de Inbox, o singură dată. O regulă de redirecționare (o regulă pentru Inbox sau o regulă de flux de corespondență, denumită și regulă de transport) poate adăuga maximum zece destinatari pentru a redirecționa un mesaj. Pentru mai multe informații, consultați [limitele regulilor pentru jurnal, transport și Inbox](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Regulile pentru Inbox nu funcționează în cutia poștală de jurnal alternativ. Pentru mai multe informații despre cutia poștală de jurnalizare alternativă, consultați [cutia poștală de jurnalizare alternativă](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Pentru a remedia aceste probleme, consultați [KB 2829319](https://support.microsoft.com/kb/2829319).

Dacă nu se aplică problemele anterioare, rulează raportul diagnostic regulă Inbox înainte de a escalada problema la asistența Microsoft:

1. Deschideți cutia poștală în Outlook pe web și faceți clic pe <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Setări**  >  **Vizualizarea tuturor setărilor Outlook**  >  **Corespondență**  >  **Reguli**.

2. În partea de jos a paginii, faceți clic pe **dacă regulile nu funcționează, faceți clic aici pentru a genera un raport de diagnosticare**.
