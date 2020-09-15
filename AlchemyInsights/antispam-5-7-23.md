---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717337"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Remedierea problemelor de livrare a mesajelor de e-mail pentru codul de eroare 5.7.23

Verificați înregistrarea SPF DNS pentru domeniul dvs., într-un verificator de înregistrare SPF sau DNS, disponibil public pe web.

Verificați dacă mesajul de ieșire nu a fost identificat ca spam de către Microsoft și a fost distribuit prin [bazinul cu risc ridicat](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Mesajele din bazinul de livrare cu risc ridicat nu vor trece de controalele SPF și, prin urmare, nu vor fi acceptate de organizația de e-mail de destinație.

Dacă problema persistă, poate fi necesar să contactați administratorul gazdei de e-mail la care încercați să trimiteți mesaje de e-mail. Notați eroarea externă detaliată disponibilă în mesajul Bounce. Asistența Microsoft poate să nu mai poată ajuta în continuare.
