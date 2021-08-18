---
title: Au primit utilizatorii dvs. mesaje de e-mail rău intenționate
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326717"
---
# <a name="did-your-users-receive-malicious-email"></a>Au primit utilizatorii dvs. mesaje de e-mail rău intenționate?

Acum puteți raporta e-mailul rău intenționat la Microsoft [utilizând Transmiteri Microsoft 365 Defender portal.](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

Mesajele care sunt [remise în remiteri](https://security.microsoft.com/reportsubmission?viewid=admin) de administrare sunt scanate și următoarele rezultate afișate în fișa detaliată:

- Dacă a existat o eroare la autentificarea prin e-mail a expeditorului în momentul livrării.
- Informații despre toate accesările de politică ce ar fi putut afecta sau înlocui verdictul unui mesaj.
- Rezultatele de detonare curente, pentru a vedea dacă adresele URL sau fișierele conținute în mesaj sunt rău intenționate sau nu.
- Feedback de la evaluatori

Dacă s-a găsit o înlocuire, rescanarea ar trebui să se termine în câteva minute. Dacă nu a existat o problemă în autentificarea prin e-mail sau dacă livrarea nu a fost afectată de o înlocuire, feedbackul de la evaluatori ar putea dura până la o zi.

Dacă nu sunteți de acord cu verdictul final pentru un mesaj, un URL sau un fișier (blocat versus neblocat), remiteți mesajul din nou a doua zi, pentru rescanare. Există șanse mari ca verdictul să se modifice după o nouă remitere a mesajului.

Între timp, puteți elimina e-mailul rău intenționat din inboxul utilizatorilor, urmând instrucțiunile din [acest articol](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Clienții cu Microsoft Defender pentru Office 365 pot:
  - Utilizarea Threat [Explorer pentru a găsi și a șterge mesajele de e-mail suspecte](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Utilizarea linkurilor Seif pentru a bloca accesul la un](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) URL rău intenționat
  - Urmărirea utilizatorilor care au făcut clic și care au accesat URL-uri rău intenționate: Vizualizați [URL-ul de înșelătorie](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)și faceți clic  &  [pe date get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Pornirea [manuală a unei investigații automate](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

De asemenea, vă puteți proteja împotriva fișierelor și URL-urilor rău intenționate, urmând instrucțiunile din [Protecție împotriva URL-urilor și fișierelor rău intenționate](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
