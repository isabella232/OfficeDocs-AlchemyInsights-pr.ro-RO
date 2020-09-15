---
title: 1332 OWA-regulile pentru Inbox nu se execută pentru o cutie poștală
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721603"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="b721a-102">O regulă de Inbox nu funcționează așa cum vă așteptați</span><span class="sxs-lookup"><span data-stu-id="b721a-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="b721a-103">Verificați următoarele setări în Outlook pe web:</span><span class="sxs-lookup"><span data-stu-id="b721a-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="b721a-104">Un mesaj poate fi Redirecționat, Redirecționat sau răspuns la automat, în funcție de regulile de Inbox, o singură dată.</span><span class="sxs-lookup"><span data-stu-id="b721a-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="b721a-105">O regulă de redirecționare (o regulă pentru Inbox sau o regulă de flux de corespondență, denumită și regulă de transport) poate adăuga maximum zece destinatari pentru a redirecționa un mesaj.</span><span class="sxs-lookup"><span data-stu-id="b721a-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="b721a-106">Pentru mai multe informații, consultați [limitele regulilor pentru jurnal, transport și Inbox](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="b721a-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="b721a-107">Regulile pentru Inbox nu funcționează în cutia poștală de jurnal alternativ.</span><span class="sxs-lookup"><span data-stu-id="b721a-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="b721a-108">Pentru mai multe informații despre cutia poștală de jurnalizare alternativă, consultați [cutia poștală de jurnalizare alternativă](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="b721a-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="b721a-109">Pentru a remedia aceste probleme, consultați [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="b721a-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="b721a-110">Dacă nu se aplică problemele anterioare, rulează raportul diagnostic regulă Inbox înainte de a escalada problema la asistența Microsoft:</span><span class="sxs-lookup"><span data-stu-id="b721a-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="b721a-111">Deschideți cutia poștală în Outlook pe web și faceți clic pe</span><span class="sxs-lookup"><span data-stu-id="b721a-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="b721a-112">**Setări**  >  **Vizualizarea tuturor setărilor Outlook**  >  **Corespondență**  >  **Reguli**.</span><span class="sxs-lookup"><span data-stu-id="b721a-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="b721a-113">În partea de jos a paginii, faceți clic pe **dacă regulile nu funcționează, faceți clic aici pentru a genera un raport de diagnosticare**.</span><span class="sxs-lookup"><span data-stu-id="b721a-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
