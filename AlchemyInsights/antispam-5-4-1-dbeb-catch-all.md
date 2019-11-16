---
title: AntiSpam 5.4.1 DBEB Catch-toate
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
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672445"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Remedierea problemelor de livrare pentru codul de eroare 550 5.4.1 Releu acces refuzat

Această problemă apare atunci când [Verificați pentru a vedea dacă o adresă de e-mail este validă pentru a preveni bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) atunci când intră în rețeaua Office 365. Încercați următoarele:

1. Determinați dacă problema este specifică unui domeniu întreg sau unei singure adrese de e-mail:
    - Domeniu întreg: uneori, domeniul trebuie să fie sincronizat; Încercați [să setarea domeniului la interne și apoi înapoi la Authoritar](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Singură adresă de e-mail: uneori, adresa trebuie să fie sincronizate; schimbarea adresei proxy SMTP și apoi schimbarea înapoi poate ajuta.
2. Determinați dacă problema este specifică unui grup sau unui folder public. Pentru unele tipuri de obiecte, obiectele pot fi necesare pentru a fi create manual în Azure Active Directory.

Dacă aveți nevoie de ajutor suplimentar, vă rugăm să deschideți un bilet de suport și să specificați domeniul de aplicare al problemei (includidng tipul de obiect pe care îl trimiteți), astfel încât să vă putem asista mai bine.