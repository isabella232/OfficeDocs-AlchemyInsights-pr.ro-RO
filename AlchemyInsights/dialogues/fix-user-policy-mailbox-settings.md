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
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="50890-102">Remedierea setărilor pentru Politica de utilizator/cutie poștală</span><span class="sxs-lookup"><span data-stu-id="50890-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="50890-103">Setările de corespondență nedorită din cutia poștală au afectat acest mesaj.</span><span class="sxs-lookup"><span data-stu-id="50890-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="50890-104">Pentru a revizui setările, procedați astfel:</span><span class="sxs-lookup"><span data-stu-id="50890-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="50890-105">Lansați componenta de administrare Exchange.</span><span class="sxs-lookup"><span data-stu-id="50890-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="50890-106">Pentru mai multe informații, consultați [Deschideți componenta de administrare Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="50890-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="50890-107">Rularea acestei comenzi (utilizând adresa de e-mail a utilizatorului):  **Get-mailboxjunkmailconfiguration-Identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="50890-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="50890-108">Verificați dacă adresa de e-mail a expeditorului face parte din **TrustedSendersAndDomains** sau **BlockedSendersAndDomains**.</span><span class="sxs-lookup"><span data-stu-id="50890-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="50890-109">Dacă adresa de e-mail se află într-una dintre liste, poate fi necesar să o eliminați.</span><span class="sxs-lookup"><span data-stu-id="50890-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="50890-110">Pentru a afla mai multe, consultați [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="50890-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
