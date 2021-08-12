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
ms.openlocfilehash: de8823253d60efcd38bfa96864c146a2cedc0537f6d0aa41de6dafc6c7debc03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929209"
---
# <a name="did-your-users-receive-malicious-email"></a>Au primit utilizatorii dvs. mesaje de e-mail rău intenționate?

- Acum puteți raporta e-mailul rău intenționat către Microsoft utilizând [Remiteri administrator din centrul de securitate și conformitate](https://sip.protection.office.com/reportsubmission).

Mesajele remise în [Remiteri administrator](https://sip.protection.office.com/reportsubmission) sunt scanate, iar următoarele rezultate sunt afișate în fișa **detalii**:

- Dacă a existat o eroare la autentificarea prin e-mail a expeditorului în momentul livrării.
- Informații despre toate accesările de politică ce ar fi putut afecta sau înlocui verdictul unui mesaj.
- Rezultatele de detonare curente, pentru a vedea dacă adresele URL sau fișierele conținute în mesaj sunt rău intenționate sau nu.
- Feedback de la evaluatori

Dacă s-a găsit o înlocuire, rescanarea ar trebui să se termine în câteva minute. Dacă nu a existat o problemă în autentificarea prin e-mail sau dacă livrarea nu a fost afectată de o înlocuire, feedbackul de la evaluatori ar putea dura până la o zi.

Dacă nu sunteți de acord cu verdictul final pentru un mesaj, un URL sau un fișier (blocat versus neblocat), remiteți mesajul din nou a doua zi, pentru rescanare. Există șanse mari ca verdictul să se modifice după o nouă remitere a mesajului.

Între timp, puteți elimina e-mailul rău intenționat din inboxul utilizatorilor, urmând instrucțiunile din [acest articol](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Clienții cu Microsoft Defender pentru Office 365 pot:
    - să utilizeze [exploratorul de amenințări pentru a găsi și a șterge e-mailul suspect](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [să utilizeze linkuri sigure pentru a bloca accesul](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) la un URL rău intenționat
    - să urmărească utilizatorii care au făcut clic și au accesat adrese URL rău intenționate: [Vizualizați URL-ul înșelător și faceți clic pe datele de verdict](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - [să inițieze o investigație automată](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office) în mod manual

De asemenea, vă puteți proteja împotriva fișierelor și URL-urilor rău intenționate, urmând instrucțiunile din [Protecție împotriva URL-urilor și fișierelor rău intenționate](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).