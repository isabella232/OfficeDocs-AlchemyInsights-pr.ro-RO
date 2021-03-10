---
title: Remedierea setărilor pentru Politica de utilizator/cutie poștală
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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695904"
---
# <a name="fix-user-policymailbox-settings"></a>Remedierea setărilor pentru Politica de utilizator/cutie poștală

Setările de corespondență nedorită din cutia poștală au afectat acest mesaj. Pentru a revizui setările, procedați astfel:

1. Lansați componenta de administrare Exchange. Pentru mai multe informații, consultați [Deschideți componenta de administrare Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Rularea acestei comenzi (utilizând adresa de e-mail a utilizatorului):  **Get-mailboxjunkmailconfiguration-Identity "user@domain.com"**
3. Verificați dacă adresa de e-mail a expeditorului face parte din **TrustedSendersAndDomains** sau **BlockedSendersAndDomains**. Dacă adresa de e-mail se află într-una dintre liste, poate fi necesar să o eliminați. Pentru a afla mai multe, consultați [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
