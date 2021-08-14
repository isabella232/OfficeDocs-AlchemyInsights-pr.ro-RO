---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932289"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Remedierea problemelor de livrare pentru codul de eroare 550 5.4.1 Acces la retransmisie refuzat

Această problemă apare atunci când [verificați dacă o adresă de e-mail](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) este validă pentru a împiedica revenirile la intrarea în rețeaua Microsoft. Încercați următoarele variante:

1. Determinați dacă problema este specifică pentru un domeniu întreg sau o singură adresă de e-mail:
    - Întregul domeniu: Uneori, domeniul trebuie să fie sincronizat; încercați [să setți domeniul la Intern, apoi înapoi la Autoritate.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Adresă de e-mail unică: uneori, adresa trebuie să fie sincronizată; changing the smtp proxy address and then changing it back can help.
2. Determinați dacă problema este specifică unui grup sau folder public. Pentru unele tipuri de obiecte, este posibil ca obiectele să fie create manual în Azure Active Directory.

Dacă aveți nevoie de ajutor suplimentar, deschideți un tichet de asistență și specificați domeniul problemei (inclusiv tipul de obiect la care trimiteți) pentru a vă putea ajuta mai bine.