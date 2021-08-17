---
title: Utilizarea DLP în regulile de transport
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
- "9002635"
- "5153"
ms.openlocfilehash: ebc0fb718eb0572e849c5d780977deaee480a00c2825c18a12e4d2212342f17a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084106"
---
# <a name="using-dlp-in-transport-rules"></a>Utilizarea DLP în regulile de transport

Pentru a integra Prevenirea pierderii datelor (DLP) într-un transport existent, utilizați condiția „**Dacă mesajul conține... Informații confidențiale**” din setarea Regulă de transport.

**Pentru mai multe detalii, consultați:**

- Tipuri de informații confidențiale DLP integrate în regulile de transport: [Integrarea regulilor pentru informații confidențiale](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

De asemenea, puteți testa regula cu sau fără testarea politicii, utilizând Modul de testare din regulă.  Înainte de a testa o regulă, ar trebui să așteptați 30 de minute după crearea acesteia.

- Consultați [Testați fluxul de corespondență/Reguli de transport](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Notă**: dacă încercați să implementați o politică DLP nouă cu regulile de transport în EAC, utilizați în schimb [Politicile DLP din Centrul de securitate și conformitate](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
