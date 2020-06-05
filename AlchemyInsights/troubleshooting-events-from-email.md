---
title: Depanarea evenimentelor din e-mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569406"
---
# <a name="troubleshooting-events-from-email"></a>Depanarea evenimentelor din e-mail

1. Verificați caracteristica este activată pentru cutia poștală: **Get-EventsFromEmailConfiguration -Identitate <mailbox> **

2. Apoi, uita-te la "Evenimente din e-mail" jurnalele **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. În jurnalele 'Evenimente din e-mail', găsiți InternetMessageId care se potrivește cu elementul din cutia poștală.  

4. Scorul de încredere determină dacă elementul este adăugat sau nu. Evenimentele vor fi adăugate numai dacă TrustScore = "Încredere".

TrustScore este determinată de proprietățile SPF, Dkim sau Dmarc, care se află în antetul mesajului.

Pentru a vizualiza aceste proprietăți:

**Discutii pe forum Windows 7**

- Deschiderea elementului
- Fișier -> Proprietăți -> anteturi Internet

Sau

**Mfcmapi**

- Navigarea la elementul din inbox
- Caută PR_TRANSPORT_MESSAGE_HEADERS_W

Aceste proprietăți sunt determinate și înregistrate în timpul transportului și dirijării. Pentru depanare suplimentară, poate fi necesar să urmăriți cu Asistență pentru transport despre defecțiunile din SPF, DKIM și.sau DMARC.