---
title: Aveți nevoie de ajutor pentru trimiterea de e-mailuri limite?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357871"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="75cc7-102">Aveți nevoie de ajutor pentru trimiterea de e-mailuri limite?</span><span class="sxs-lookup"><span data-stu-id="75cc7-102">Need help with email sending limits?</span></span>

<span data-ttu-id="75cc7-103">Mai jos este **de-design trimiterea limitelor** aplicate în serviciu.</span><span class="sxs-lookup"><span data-stu-id="75cc7-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="75cc7-104">Mai multe informații cu privire la aceste limite sunt documentate [aici](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="75cc7-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="75cc7-105">Pentru a descuraja livrarea de mesaje în bloc nesolicitate, aplicăm limitele de rată ale **destinatarului**per utilizator tuturor mesajelor de ieșire și interne .</span><span class="sxs-lookup"><span data-stu-id="75cc7-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="75cc7-106">În toate SKU-urile, această limită este **de 10.000 de destinatari pe zi.**</span><span class="sxs-lookup"><span data-stu-id="75cc7-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="75cc7-107">Clienții care trebuie să trimită e-mailuri comerciale în bloc legitime (de exemplu, buletine informative pentru clienți) ar trebui să utilizeze furnizori terți specializați în aceste servicii.</span><span class="sxs-lookup"><span data-stu-id="75cc7-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="75cc7-108">**Notă:** Odată ce limita de rată a destinatarului este atinsă, mesajele nu pot fi trimise din cutia poștală până când numărul de destinatari cărora le-au fost trimise mesaje în ultimele 24 de ore scade sub limită.</span><span class="sxs-lookup"><span data-stu-id="75cc7-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="75cc7-109">Utilizatorul nu va putea trimite mesaje până în acel moment.</span><span class="sxs-lookup"><span data-stu-id="75cc7-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="75cc7-110">Limita ratei de mesaj de **30 de mesaje pe minut** se aplică în toate SKU-uri.</span><span class="sxs-lookup"><span data-stu-id="75cc7-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="75cc7-111">Acest lucru determină câte mesaje poate trimite un utilizator din contul exchange online într-o perioadă specificată.</span><span class="sxs-lookup"><span data-stu-id="75cc7-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="75cc7-112">**Numărul maxim de destinatari permis în câmpurile Către, Cc și Cci** pentru un singur mesaj de poștă electronică, în toate SKU-urile, este de **1000 de destinatari**.</span><span class="sxs-lookup"><span data-stu-id="75cc7-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="75cc7-113">Pentru a particulariza această limită, mergeți [aici](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="75cc7-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
