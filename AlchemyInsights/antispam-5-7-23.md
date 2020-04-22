---
title: Antispam - 5.7.23
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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676509"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Remediați problemele de livrare de e-mail pentru codul de eroare 5.7.23

Verificați înregistrarea SPF DNS pentru domeniul dvs., la un verificatorul de înregistrări SPF sau DNS disponibil publicului pe web.

Verificați dacă mesajul de ieșire nu a fost identificat ca spam de microsoft și distribuit prin [rezervorul de livrare cu risc ridicat](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Mesajele din rezervorul de livrare cu risc ridicat nu vor trece de verificările SPF și, prin urmare, nu vor fi acceptate de organizația de e-mail de destinație.

Dacă problema persistă, poate fi necesar să contactați administratorul gazdei de e-mail la care încercați să trimiteți e-mailuri. Notați eroarea externă detaliată disponibilă în mesajul de respingere. Este posibil ca asistența Microsoft să nu poată fi asistată în continuare.
