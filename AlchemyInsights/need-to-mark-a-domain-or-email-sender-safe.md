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
ms.openlocfilehash: 57d1e2d696a8be42b5f868f021d829bf019349bf
ms.sourcegitcommit: 3994cece80410371330b39f7b79b1b1c1bfcf648
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/08/2021
ms.locfileid: "52286692"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Trebuie să marcați un domeniu sau un expeditor de e-mail ca sigur?

- Utilizarea **listelor de expeditori siguri** nu este recomandată, deoarece deschide organizația dvs. în atacuri de spam, fals și fals fals.
- Cu toate acestea, dacă există o cerință de afaceri, **vă recomandăm să** utilizați **[Regulile de Flow corespondenței](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pentru acest lucru. Instrucțiunile noastre asigură autentificarea expeditorului (verificarea domeniului de trimitere nu este falsificată). **Notă:** Nu recomandăm gestionarea fals pozitive utilizând listele de expeditori siguri, deoarece excepțiile de la filtrarea antispam pot deschide organizația dvs. la atacuri de securitate. Dacă utilizatorii dvs. primesc mesaje marcate incorect ca spam sau e-mailuri nedorite, **[raportați mesajele și fișierele la Microsoft](https://protection.office.com/reportsubmission)**.
- Seif Expeditorii din Outlook, lista de expeditori permiteți sau lista  de domenii permise din politicile antispam trebuie evitate, deoarece expeditorii ocolesc tot spamul, falsoful și protecția antispam și autentificarea expeditorului (SPF, DKIM, DMARC). Această metodă se utilizează cel mai bine numai pentru testarea temporară.
- Validarea faptul că o anumită evaluare de e-mail ocolește Antispam poate fi efectuată dacă verificați antetul mesajului "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN), consultați **[Anteturile mesajelor antispam.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Întrucât Microsoft dorește să-și păstreze clienții [în siguranță în mod](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)implicit, unele înlocuiri ale entităților găzduite nu sunt aplicate pentru malware și phishing cu încredere ridicată. Printre aceste înlocuiri se numără: o Liste de expeditori permiteți sau liste de domenii permise (politici antispam) sau Outlook Seif Expeditori sau Listă de adrese IP permise (filtrarea conexiunii) 
- Singura înlocuire care permite mesajelor de înșelăciune de încredere să ocolească filtrarea este Exchange de flux de corespondență (cunoscute și ca reguli de transport). Pentru a utiliza reguli de flux de corespondență pentru a ocoli filtrarea, consultați Utilizarea regulilor de flux de corespondență pentru a seta nivelul de încredere **[pentru spam (SCL) în mesaje.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**