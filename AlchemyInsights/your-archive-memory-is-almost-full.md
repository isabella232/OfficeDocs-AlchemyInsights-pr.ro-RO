---
title: Cutia poștală de arhivă este aproape completă
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974661"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Cutia poștală de arhivă este aproape completă

Dacă utilizatorul primește avertismentul; **Cutia poștală de arhivă este aproape completă** sau trebuie să măriți dimensiunea cutiei poștale de arhivă, iată câteva sfaturi:

1. Dacă utilizatorului i se atribuie un plan Exchange Online 1, faceți upgrade la licența **Exchange Online Plan 2** pentru a mări dimensiunea de la 50 GB la 100 GB.
1. Dacă utilizatorul este deja atribuit oricare dintre următoarele: **Exchange Online Plan 2** sau un Exchange Online plan 1 cu un program de completare Arhivare Exchange Online, utilizați pașii de mai jos pentru a activa Arhivarea automată a extinderii:.
 
    1. [Conectați-vă la Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Rulează următorul poate configura utilizând pentru utilizator:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Rularea următoarelor poate configura utilizând pentru a confirma că este activată pentru utilizator:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Pentru mai multe informații, consultați:

- [ Activarea Arhivării nelimitate-ajutor pentru administratori-Microsoft 365 Conformity | Documente Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Limitele Exchange Online-descrierile serviciului | Documente Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Upgrade-ul la un alt plan de afaceri | Documente Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

