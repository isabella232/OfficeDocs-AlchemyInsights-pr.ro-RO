---
title: Nu se poate trimite/primi mesaje de e-mail la/de la Office 365 din cauza indisponibilității TLS 1,0 și TLS 1,1
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
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747119"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Nu se poate trimite/primi mesaje de e-mail la/de la Office 365 din cauza indisponibilității TLS 1,0 și TLS 1,1

Așa cum s-a confirmat de mesajul post Center MC229914, TLS 1,0 și TLS 1,1 au început impunerea pentru punctele finale pentru fluxul de corespondență Exchange Online. În curând Office 365 nu va mai accepta conexiuni de e-mail TLS 1,0 și TLS 1,1 din surse externe. De asemenea, Exchange Online nu va utiliza niciodată TLS 1,0 sau 1,1 pentru a trimite mesaje de e-mail de ieșire. Dacă întâmpinați probleme din cauza unei dezreușite TLS 1,0 sau 1,1, este posibil să vă confruntați cu una dintre următoarele erori-

- Expeditorul devine NDR Bounce back-' 421 4.4.2 conexiune retrasă din cauza SocketError '
- Eroare în vizualizatorul de cozi al serverului local, care trimite mesaje de e-mail către ofițer 365-' 421 conexiune 4.4.2 retrasă din cauza SocketError '
- Eroare în Jurnalul de [protocoale](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) trimitere conector de pe serverul care trimite mesaje de E-mail la Office 365-TLS negociere nereușită cu eroarea SocketError
- Eroare în Jurnalul de protocoale trimitere sau primire-' 451 5.7.3 trebuie să emită o comandă STARTTLS mai întâi '

Dacă întâmpinați oricare dintre erorile de mai sus, asigurați-vă că serverul care trimite sau primește mesaje de e-mail are TLS 1,2 activat, verificând următoarele chei de registry-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ client] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ server] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001**

Dacă efectuați modificări în cheile de registry de mai sus pentru a activa TLS 1,2, reporniți serverul pentru ca modificările să aibă efect. De asemenea, asigurați-vă că aveți instalate cele mai recente actualizări Windows și Exchange.

Pentru mai multe informații, consultați:

- [Orientare Exchange Server TLS, partea 1: pregătirea pentru TLS 1,2-comunitatea tehnică Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Partea de orientare Exchange Server TLS 2: Activarea TLS 1,2 și identificarea clienților care nu îl utilizează-comunitatea Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Înțelegerea scenariilor de e-mail dacă versiunile TLS nu pot fi aprobate cu Exchange Online-comunitatea Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
