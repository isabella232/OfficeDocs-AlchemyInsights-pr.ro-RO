---
title: Aveți nevoie de ajutor pentru limitele de trimitere a mesajelor de e-mail?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836291"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="b1c83-102">Aveți nevoie de ajutor pentru limitele de trimitere a mesajelor de e-mail?</span><span class="sxs-lookup"><span data-stu-id="b1c83-102">Need help with email sending limits?</span></span>

<span data-ttu-id="b1c83-103">Mai jos sunt **limitele de trimitere proiectate** impuse în serviciu.</span><span class="sxs-lookup"><span data-stu-id="b1c83-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="b1c83-104">Mai multe informații despre aceste limite sunt documentate [aici](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="b1c83-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="b1c83-105">Pentru a descuraja livrarea mesajelor în masă nesolicitate, aplicăm pe utilizator **limite pentru la rata de destinatari la toate mesajele de ieșire și cele interne**.</span><span class="sxs-lookup"><span data-stu-id="b1c83-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="b1c83-106">În toate SKU-urile, această limită este de **10.000 de destinatari pe zi**.</span><span class="sxs-lookup"><span data-stu-id="b1c83-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="b1c83-107">Clienții care trebuie să trimită mesaje de e-mail comerciale în masă legitime (de exemplu, buletine informative pentru clienți), trebuie să utilizeze furnizori terți specializați în aceste servicii.</span><span class="sxs-lookup"><span data-stu-id="b1c83-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="b1c83-108">**Notă**: După ce s-a atins limita de destinatari, nu pot fi trimise mesaje din cutia poștală decât după ce numărul de destinatari cărora li s-au trimis mesaje în ultimele 24 de ore scade sub limită.</span><span class="sxs-lookup"><span data-stu-id="b1c83-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="b1c83-109">Utilizatorul nu va putea trimite mesaje până în acel moment.</span><span class="sxs-lookup"><span data-stu-id="b1c83-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="b1c83-110">Limita ratei de mesaje de **30 de mesaje pe minut** se aplică în toate SKU-urile.</span><span class="sxs-lookup"><span data-stu-id="b1c83-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="b1c83-111">Acest lucru determină câte mesaje poate trimite un utilizator din contul său Exchange Online într-un anumit interval de timp.</span><span class="sxs-lookup"><span data-stu-id="b1c83-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="b1c83-112">**Numărul maxim permis de destinatari în câmpurile Către, Cc și Cci** pentru un singur mesaj de e-mail, în toate SKU-urile, este de **1000 de destinatari**.</span><span class="sxs-lookup"><span data-stu-id="b1c83-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="b1c83-113">Pentru a particulariza această limită, mergeți [aici](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="b1c83-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
