---
title: Remedierea politicii de utilizator/setărilor cutiei poștale
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034730"
---
# <a name="fix-user-policymailbox-settings"></a>Remedierea politicii de utilizator/setărilor cutiei poștale

Setările de corespondență nedorită din cutia poștală au afectat acest mesaj. Pentru a examina setările, acțiunile următoare:

1. Lansați Exchange de administrare. Pentru mai multe informații, [consultați Deschiderea Exchange de administrare .](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Rulați această comandă (utilizând adresa de e-mail a utilizatorului):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Verificați dacă adresa de e-mail a expeditorului face parte din **TrustedSendersAndDomains** **sau BlockedSendersAndDomains.** Dacă adresa de e-mail este într-una dintre liste, poate fi necesar să o eliminați. Pentru a afla mai multe, [consultați Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
