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
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381860"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="594e4-102">Rezervor retransmisie de ieșire</span><span class="sxs-lookup"><span data-stu-id="594e4-102">Outbound relay pool</span></span>

<span data-ttu-id="594e4-103">Microsoft face câteva modificări în configurația de trimitere sau redirecționare a e-mailului prin Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="594e4-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="594e4-104">Mesajele din anumite scenarii sunt redirecționate sau retransmise prin Microsoft 365 utilizând un rezervor de retransmisie special.</span><span class="sxs-lookup"><span data-stu-id="594e4-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="594e4-105">Mesajele trimise prin utilizarea rezervorului de retransmisie pot ajunge în folderul de corespondență nedorită al destinatarului.</span><span class="sxs-lookup"><span data-stu-id="594e4-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="594e4-106">Pentru mai multe informații, consultați [Fonduri de livrare de ieșire](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="594e4-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="594e4-107">Pentru a evita un scenariu utilizând retransmisia, asigurați-vă că mesajele redirecționate/retransmise îndeplinesc unul dintre criteriile următoare:</span><span class="sxs-lookup"><span data-stu-id="594e4-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="594e4-108">Expeditorul de ieșire este un domeniu acceptat al entității găzduite.</span><span class="sxs-lookup"><span data-stu-id="594e4-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="594e4-109">Sender Policy Framework (SPF) trece atunci când mesajul ajunge la Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="594e4-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="594e4-110">DomainKeys Identified Mail (DKIM) pe domeniul de expeditor P2 trece atunci când mesajul ajunge la Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="594e4-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="594e4-111">Mesajele care îndeplinesc criteriile de mai sus nu sunt retransmise prin intermediul rezervorului de retransmisie.</span><span class="sxs-lookup"><span data-stu-id="594e4-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="594e4-112">Dacă înregistrarea MX pentru domeniul dvs. este trimisă la un server terț sau local, utilizați filtrarea îmbunătățită pentru a vă asigura că validarea SPF este corectă pentru e-mailul de intrare și pentru a evita trimiterea de mesaje de e-mail prin retransmisie.</span><span class="sxs-lookup"><span data-stu-id="594e4-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="594e4-113">**Cum ne putem da seama dacă suntem afectați de releu?**</span><span class="sxs-lookup"><span data-stu-id="594e4-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="594e4-114">Dacă mesajele de e-mail redirecționate sau retransmise utilizează unul dintre criteriile de mai sus, mesajele nu vor fi retransmise prin intermediul rezervorului de retransmisie.</span><span class="sxs-lookup"><span data-stu-id="594e4-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="594e4-115">Cu toate acestea, dacă un mesaj este trimis printr-un rezervor de retransmisie, IP-ul serverului de ieșire se află în zona 40.95.0.0/16, iar numele serverului de ieșire include **rly** în nume.</span><span class="sxs-lookup"><span data-stu-id="594e4-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

