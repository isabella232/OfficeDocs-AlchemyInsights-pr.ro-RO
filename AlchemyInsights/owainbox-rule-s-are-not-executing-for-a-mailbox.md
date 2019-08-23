---
title: 1332 OWA - Inbox rule(s) sunt nu executa pentru o cutie poştală
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 901237d4dc7b99695097142c61a4bfef7c09750d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36555785"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="769b9-102">Regulă Inbox nu funcţionează conform aşteptărilor</span><span class="sxs-lookup"><span data-stu-id="769b9-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="769b9-103">Verificaţi următoarele setări în Outlook pe web:</span><span class="sxs-lookup"><span data-stu-id="769b9-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="769b9-104">Un mesaj poate fi redirecţionat, altui tip de conþinut, sau a răspuns la automat bazat pe reguli Inbox numai o singură dată.</span><span class="sxs-lookup"><span data-stu-id="769b9-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="769b9-105">O regulă de redirecţionare (o regulă Inbox sau mail fluxul de regulă, de asemenea, cunoscut ca o regulă de transport) puteţi adăuga maximum zece expediere destinatari la un mesaj.</span><span class="sxs-lookup"><span data-stu-id="769b9-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="769b9-106">Pentru informaţii suplimentare, consultaţi [jurnal, Transport, şi Inbox limitele de regula](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="769b9-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="769b9-107">Regulile pentru Inbox nu funcţionează pe cutia poştală de jurnalizare alternativ.</span><span class="sxs-lookup"><span data-stu-id="769b9-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="769b9-108">Pentru mai multe informaţii despre cutia poştală de jurnalizare alternativă, a se vedea [poştală de jurnalizare alternativ](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="769b9-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="769b9-109">Pentru a rezolva aceste probleme, a se vedea [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="769b9-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="769b9-110">În cazul în care problemele anterioare nu se aplică, executaţi raportul regulă Inbox de diagnosticare înainte să escaladeze emiterii către Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="769b9-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="769b9-111">Deschide cutia poştală în Outlook pe web, şi faceţi clic pe</span><span class="sxs-lookup"><span data-stu-id="769b9-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="769b9-112">**Setări** > **Vezi toate setările de Outlook** > **Mail** > **reguli**.</span><span class="sxs-lookup"><span data-stu-id="769b9-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="769b9-113">În partea de jos a paginii, faceţi clic pe **dacă regulile tale nu sunt de lucru faceţi clic aici pentru a genera un raport de diagnostic**.</span><span class="sxs-lookup"><span data-stu-id="769b9-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
