---
title: Trebuie să marcați un domeniu sau un expeditor de e-mail ca sigur?
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
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792144"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Trebuie să marcați un domeniu sau un expeditor de e-mail ca sigur?

- Utilizarea **listelor de expeditori siguri** nu este recomandată, deoarece deschide organizația dvs. în atacuri de spam, fals și fals fals.
- Cu toate acestea, dacă există o cerință de afaceri, vă **recomandăm să utilizați** reguli de flux de **[corespondență](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pentru acest lucru. Instrucțiunile noastre asigură autentificarea expeditorului (verificarea domeniului de trimitere nu este falsificată). **Notă:** Nu recomandăm gestionarea fals pozitive utilizând listele de expeditori siguri, deoarece excepțiile de la filtrarea antispam pot deschide organizația dvs. la atacuri de securitate. Dacă utilizatorii dvs. primesc mesaje marcate incorect ca spam sau e-mailuri nedorite, **[raportați mesajele și fișierele la Microsoft](https://protection.office.com/reportsubmission)**.
- Expeditorii siguri din Outlook, lista de expeditori blocați  sau lista de domenii permise din politicile antispam trebuie evitate, deoarece expeditorii ocolesc tot spamul, falsoful și protecția antispam și autentificarea expeditorului (SPF, DKIM, DMARC). Această metodă se utilizează cel mai bine numai pentru testarea temporară.
