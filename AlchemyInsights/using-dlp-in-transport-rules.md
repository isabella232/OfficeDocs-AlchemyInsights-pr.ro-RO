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
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827228"
---
# <a name="using-dlp-in-transport-rules"></a>Utilizarea DLP în regulile de transport

Pentru a integra Prevenirea pierderii datelor (DLP) într-un transport existent, utilizați condiția „**Dacă mesajul conține... Informații confidențiale**” din setarea Regulă de transport.

**Pentru mai multe detalii, consultați:**

- Tipuri de informații confidențiale DLP integrate în regulile de transport: [Integrarea regulilor pentru informații confidențiale](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

De asemenea, puteți testa regula cu sau fără testarea politicii, utilizând Modul de testare din regulă.  Înainte de a testa o regulă, ar trebui să așteptați 30 de minute după crearea acesteia.

- Consultați [Testați fluxul de corespondență/Reguli de transport](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Notă**: dacă încercați să implementați o politică DLP nouă cu regulile de transport în EAC, utilizați în schimb [Politicile DLP din Centrul de securitate și conformitate](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
