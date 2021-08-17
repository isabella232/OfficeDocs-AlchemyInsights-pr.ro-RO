---
title: Depanarea evenimentelor din e-mail
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
- "9000301"
- "5765"
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105364"
---
# <a name="troubleshooting-events-from-email"></a>Depanarea evenimentelor din e-mail

1. Verificați dacă este activată caracteristica pentru cutia poștală: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Apoi, verificați jurnalele "Evenimente din **e-mail" Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. În jurnalele "Evenimente din e-mail", găsiți InternetMessageId care se potrivește cu elementul din cutia poștală.  

4. TrustScore determină dacă elementul este adăugat sau nu. Evenimentele vor fi adăugate doar dacă TrustScore = "Trusted".

TrustScore este determinată de proprietățile SPF, Dkim sau Dmarc, care se află în Antetul mesajului.

Pentru a vizualiza aceste proprietăți:

**Desktop Outlook**

- Deschideți elementul
- File -> Properties -> Anteturi Internet

sau

**MFCMapi**

- Navigarea la elementul din inbox
- Căutați un PR_TRANSPORT_MESSAGE_HEADERS_W

Aceste proprietăți sunt determinate și înregistrate în timpul transportului și direcționării. Pentru depanare suplimentară, poate fi necesar să continuați cu asistența pentru transport cu privire la erorile din SPF, DKIM și.or DMARC.