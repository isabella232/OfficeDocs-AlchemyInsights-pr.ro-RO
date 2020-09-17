---
title: Doriți să marcați în siguranță un domeniu sau un expeditor de e-mail?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803257"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Doriți să marcați în siguranță un domeniu sau un expeditor de e-mail?

- Utilizarea **listelor de expeditori siguri nu este recomandată** , deoarece vă deschide organizația la atacuri spam, phishing și falsificare.
- Cu toate acestea, dacă există o cerință de afaceri, vă **recomandăm** să utilizați **[regulile de flux de corespondență](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pentru aceasta. Ghidul nostru asigură autentificarea expeditorului (verifică dacă trimiterea domeniului nu este falsificată). **Notă**: nu recomandăm gestionarea unor valori false pozitive utilizând listele de expeditori siguri, deoarece excepțiile de la Filtrarea antispam pot deschide organizația la atacuri de securitate. Dacă utilizatorii primesc mesaje marcate incorect ca spam sau e-mailuri nedorite, **[Raportați mesaje și fișiere la Microsoft](https://protection.office.com/reportsubmission)**.
- Expeditorii siguri din Outlook, lista Expeditori acceptați sau lista de domenii permise în politicile anti-spam **trebuie evitate** , deoarece expeditorii ocolesc toate protecția antispam, spoof și phishing și autentificarea expeditorului (SPF, DKIM, DMARC). Această metodă este utilizată cel mai bine doar pentru testarea temporară.
