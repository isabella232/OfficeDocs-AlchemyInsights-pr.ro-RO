---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682256"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Fix probleme de livrare e-mail pentru codul de eroare 5.7.23

Verificați înregistrarea SPF DNS pentru domeniu la un verificator de înregistrări SPF sau DNS disponibile public pe web.

Verificați că mesajul de ieșire nu a fost identificat ca spam de Office 365 și rutate prin [rezervorul de livrare de risc ridicat](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Mesajele din rezervorul de livrare cu risc ridicat nu vor trece de controalele SPF și, prin urmare, nu vor fi acceptate de organizația de e-mail de destinație.

Dacă problema persistă, poate fi necesar să contactați administratorul gazdă de poștă electronică la care încercați să trimiteți e-mailuri. Notați eroarea externă detaliată disponibilă în mesajul de respingere.  Este posibil ca asistența Office 365 să nu poată asista în continuare.