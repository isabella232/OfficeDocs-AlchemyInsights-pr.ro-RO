---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932181"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Remediați problemele de livrare a mesajelor de e-mail pentru codul de eroare 5.7.23

Verificați înregistrarea DNS SPF pentru domeniul dvs. la un verificator de înregistrări SPF sau DNS disponibil public pe web.

Verificați dacă mesajul de ieșire nu a fost identificat ca spam de către Microsoft și distribuit prin intermediul [rezervorului de livrare pentru risc înalt.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Mesajele din rezervor de livrare cu risc înalt nu vor trece verificările SPF și, prin urmare, nu vor fi acceptate de organizația de e-mail de destinație.

Dacă problema persistă, poate fi necesar să contactați administratorul gazdei de e-mail la care încercați să trimiteți e-mail. Rețineți eroarea externă detaliată disponibilă în mesajul returnat. Asistența Microsoft ar putea să nu vă mai poată ajuta.
