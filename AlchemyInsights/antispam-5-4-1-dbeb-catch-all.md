---
title: AntiSpam 5.4.1 DBEB captură-toate
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717373"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Remedierea problemelor de livrare pentru codul de eroare 550 5.4.1 Releu Access Denied

Această problemă apare atunci când [Căutați pentru a vedea dacă o adresă de e-mail este validă pentru a împiedica bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) atunci când introduceți rețeaua Microsoft. Încercați următoarele:

1. Determinați dacă problema este specifică pentru un domeniu întreg sau pentru o singură adresă de e-mail:
    - Domeniu întreg: uneori, domeniul trebuie sincronizat; Încercați să [Setați domeniul la intern, apoi înapoi la autoritate](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Adresă de e-mail unică: uneori, adresa trebuie sincronizată; Modificarea adresei proxy SMTP, apoi modificarea sa înapoi vă poate ajuta.
2. Determinați dacă problema este specifică pentru un grup sau un folder public. Pentru unele tipuri de obiecte, este posibil ca obiectele să trebuiască să fie create manual în Azure Active Directory.

Dacă aveți nevoie de ajutor suplimentar, vă rugăm să deschideți un tichet de asistență și să specificați domeniul problemei (inclusiv tipul de obiect pe care îl trimiteți) pentru a vă putea ajuta mai bine.