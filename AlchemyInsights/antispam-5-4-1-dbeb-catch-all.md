---
title: AntiSpam 5.4.1 DBEB catch-all AntiSpam 5.4.1 DBEB catch-all AntiSpam 5.4.1 DBEB catch-all AntiSpam
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707923"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Remedierea problemelor de livrare pentru codul de eroare 550 5.4.1 Releu de acces refuzat

Această problemă apare atunci când [verificați pentru a vedea dacă o adresă de poștă electronică este validă pentru a preveni bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) atunci când intră în rețeaua Microsoft. Încercați următoarele:

1. Determinați dacă problema este specifică unui domeniu întreg sau unei singure adrese de e-mail:
    - Domeniu întreg: Uneori, domeniul trebuie sincronizat; încercați [să setezeți domeniul la intern și apoi înapoi la autoritate](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Adresă de e-mail unică: Uneori, adresa trebuie sincronizată; schimbarea adresei proxy smtp și apoi schimbarea-l înapoi poate ajuta.
2. Determinați dacă problema este specifică unui grup sau unui folder public. Pentru unele tipuri de obiecte, obiectele poate fi necesar să fie create manual în Azure Active Directory.

Dacă aveți nevoie de ajutor suplimentar, deschideți un bilet de asistență și specificați domeniul de aplicare al problemei (inclusiv tipul de obiect la care trimiteți), astfel încât să vă putem ajuta mai bine.