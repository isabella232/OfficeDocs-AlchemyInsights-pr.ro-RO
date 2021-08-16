---
title: Cutia poștală de arhivare este aproape plină
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046764"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Cutia poștală de arhivare este aproape plină

Dacă utilizatorul primește avertismentul; **Cutia poștală de arhivare este** aproape plină sau trebuie să măriți dimensiunea cutiei poștale de arhivare, iată câteva sfaturi:

1. Dacă utilizatorului i se atribuie o licență Exchange Online Plan 1, faceți upgrade la **Exchange Online Plan 2** pentru a mări dimensiunea de la 50 GB la 100 GB.
1. Dacă utilizatorului i se atribuie deja unul dintre următoarele: **Exchange Online Plan 2** sau un Exchange Online Plan 1 cu un program de completare Arhivare Exchange Online, utilizați pașii de mai jos pentru a activa arhivarea automată:
 
    1. [Conectare la Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Rulați următorul commandlet pentru utilizator:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Rulați următorul commandlet pentru a confirma că este activat pentru utilizator:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Pentru mai multe informații, consultați:

- [Activați arhivarea nelimitată - Ajutor pentru administratori - Microsoft 365 de | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online limite - Descrierea serviciului | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Upgrade-ul la un alt plan | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

