---
title: Rezervor retransmisie de ieșire
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326089"
---
# <a name="outbound-relay-pool"></a>Rezervor retransmisie de ieșire

Microsoft face câteva modificări în configurația de trimitere sau redirecționare a e-mailului prin Microsoft 365. Mesajele din anumite scenarii sunt redirecționate sau retransmise prin Microsoft 365 utilizând un rezervor de retransmisie special. Mesajele trimise prin utilizarea rezervorului de retransmisie pot ajunge în folderul de corespondență nedorită al destinatarului. Pentru mai multe informații, consultați [Fonduri de livrare de ieșire](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Pentru a evita un scenariu utilizând retransmisia, asigurați-vă că mesajele redirecționate/retransmise îndeplinesc unul dintre criteriile următoare:

- Expeditorul de ieșire este un domeniu acceptat al entității găzduite.
- Sender Policy Framework (SPF) trece atunci când mesajul ajunge la Microsoft 365.
- DomainKeys Identified Mail (DKIM) de pe domeniul P2 sender trece atunci când mesajul ajunge la Microsoft 365.
 
Mesajele care îndeplinesc criteriile de mai sus nu sunt retransmise prin intermediul rezervorului de retransmisie.

Dacă înregistrarea MX pentru domeniul dvs. este trimisă la un server terț sau local, utilizați filtrarea îmbunătățită pentru a vă asigura că validarea SPF este corectă pentru e-mailurile de intrare și pentru a evita trimiterea de mesaje de e-mail prin retransmisie.

**Cum ne putem da seama dacă suntem afectați de releu?**

Dacă mesajele de e-mail redirecționate sau retransmise utilizează unul dintre criteriile de mai sus, mesajele nu vor fi retransmise prin intermediul rezervorului de retransmisie. Cu toate acestea, dacă un mesaj este trimis printr-un rezervor de retransmisie, IP-ul serverului de ieșire se află în zona 40.95.0.0/16, iar numele serverului de ieșire include **rly** în nume.

