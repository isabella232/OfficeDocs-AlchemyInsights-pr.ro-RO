---
title: Depanarea evenimentelor din E-mail
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
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658746"
---
# <a name="troubleshooting-events-from-email"></a>Depanarea evenimentelor din E-mail

1. Verificați dacă este activată caracteristica pentru cutia poștală: **Get-EventsFromEmailConfiguration <mailbox> -Identity**

2. Apoi, uitați-vă la "evenimente din e-mailul" jurnalele de **Export-MailboxDiagnosticLogs <mailbox> -componenta TimeProfile**

3. În jurnalele "evenimente din E-mail", găsiți InternetMessageId care se potrivește cu elementul din cutia poștală.  

4. TrustScore determină dacă elementul este adăugat sau nu. Evenimentele vor fi adăugate doar dacă TrustScore = "de încredere".

TrustScore este determinată de proprietățile SPF, DKIM sau DMARC, care se află în antetul mesajului.

Pentru a vizualiza aceste proprietăți:

**Outlook pentru desktop**

- Deschiderea elementului
- Fișier-> proprietăți-> anteturi de Internet

sau

**MFCMapi**

- Navigarea la elementul din Inbox
- Căutați PR_TRANSPORT_MESSAGE_HEADERS_W

Aceste proprietăți sunt determinate și înregistrate în timpul transportului și rutare. Pentru depanarea ulterioară, poate fi necesar să urmăriți asistența pentru transport cu privire la erorile din SPF, DKIM și. or DMARC.