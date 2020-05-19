---
title: Trebuie să marcați un domeniu sau un expeditor de e-mail în siguranță?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281183"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Trebuie să marcați un domeniu sau un expeditor de e-mail în siguranță?

- Utilizarea listelor de **expeditori siguri nu este recomandată,** deoarece deschide organizația la atacuri spam, phish și falsificare.
- Cu toate acestea, dacă există o cerință de afaceri, **vă recomandăm să** utilizați **[Reguli flux de corespondență](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pentru acest lucru. Ghidul nostru asigură autentificarea expeditorului (verifică trimiterea domeniului nu este falsificată). **Notă:** Nu recomandăm gestionarea informațiilor fals pozitive utilizând liste de expeditori siguri, deoarece excepțiile de la filtrarea spamului vă pot deschide organizația la atacuri de securitate. Dacă utilizatorul (utilizatorii) primesc mesaje marcate incorect ca spam sau e-mail nedorit, **[raportați mesaje și fișiere la Microsoft](https://protection.office.com/reportsubmission)**.
- Expeditorii siguri din Outlook, lista de expeditori permise sau lista de domenii permisă în politicile anti-spam **trebuie evitate,** deoarece expeditorii ocolesc toate mesajele spam, lingură și protecția phish și autentificarea expeditorului (SPF, DKIM, DMARC). Această metodă este cel mai bine utilizată numai pentru testarea temporară.
