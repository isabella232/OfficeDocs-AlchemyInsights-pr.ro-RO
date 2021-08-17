---
title: Nu puteți să trimiteți/să primiți e-mail la/de Office 365 din cauza dezactivării TLS 1.0 și TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054918"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Nu puteți să trimiteți/să primiți e-mail la/de Office 365 din cauza dezactivării TLS 1.0 și TLS 1.1

După cum a confirmat centrul de mesaje, postarea MC229914, TLS 1.0 și perimarea TLS 1.1 a început să se impune pentru Exchange Online puncte finale de flux de corespondență. În Office 365 va mai accepta conexiuni de e-mail TLS 1.0 și TLS 1.1 de la surse externe. De asemenea, Exchange Online va utiliza niciodată TLS 1.0 sau 1.1 pentru a trimite mesaje de e-mail de ieșire. Dacă vă confruntați cu probleme din cauza dezactivării TLS 1.0 sau 1.1, este posibil să vă confruntați cu una dintre următoarele erori:

- Expeditorul obține NDR returnat - "421 4.4.2 Conexiunea a fost retrasă din cauza SocketError"
- Eroare în Vizualizatorul de coadă de așteptare al serverului local care trimite e-mail la Officer 365- '421 4.4.2 Conexiunea a fost retrasă din cauza SocketError'
- Eroare în jurnalul Send connector [Protocol de](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) pe server care trimite e-mail la Office 365 - Negocierea TLS a eșuat cu eroarea SocketError
- Eroare în jurnalul de protocol Trimitere sau primire conector - "451 5.7.3 Trebuie să emită mai întâi o comandă STARTTLS"

Dacă vă experimentați oricare dintre erorile de mai sus, asigurați-vă că serverul care trimite sau primește e-mail are TLS 1.2 activat verificând următoarele chei de registry-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Dacă efectuați orice modificare în cheile de registry de mai sus pentru a activa TLS 1.2, reporniți serverul pentru ca modificările să aibă efect. De asemenea, asigurați-vă că aveți cele mai Windows și cele Exchange instalate actualizări.

Pentru mai multe informații, consultați:

- [Exchange Server Instrucțiuni TLS, partea 1: Pregătiți-vă pentru TLS 1.2 - Comunitatea tehnică Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server Instrucțiuni TLS, partea 2: Activarea TLS 1.2 și identificarea clienților care nu o utilizează - Comunitatea tehnică Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Înțelegerea scenariilor de e-mail în cazul în care versiunile TLS nu pot fi aprobate cu Exchange Online - Comunitatea tehnică Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
