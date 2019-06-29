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
ms.openlocfilehash: 7d1848830847fc6722da20e09a4875f49bf02bd3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35360929"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="a9cc0-102">Regulă Inbox nu funcţionează conform aşteptărilor</span><span class="sxs-lookup"><span data-stu-id="a9cc0-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="a9cc0-103">Verificaţi următoarele setări:</span><span class="sxs-lookup"><span data-stu-id="a9cc0-103">Verify the following settings:</span></span>

- <span data-ttu-id="a9cc0-104">Un mesaj poate fi redirecţionat, altui tip de conþinut, sau a răspuns la automat bazat pe reguli Inbox numai o singură dată.</span><span class="sxs-lookup"><span data-stu-id="a9cc0-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="a9cc0-105">O regulă de redirecţionare (o regulă Inbox sau mail fluxul de regulă, de asemenea, cunoscut ca o regulă de transport) puteţi adăuga maximum zece expediere destinatari la un mesaj.</span><span class="sxs-lookup"><span data-stu-id="a9cc0-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="a9cc0-106">Pentru informaţii suplimentare, consultaţi [jurnal, Transport, şi Inbox limitele de regula](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="a9cc0-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="a9cc0-107">Regulile pentru Inbox nu funcţionează pe cutia poştală de jurnalizare alternativ.</span><span class="sxs-lookup"><span data-stu-id="a9cc0-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="a9cc0-108">Pentru mai multe informaţii despre cutia poştală de jurnalizare alternativă, a se vedea [poştală de jurnalizare alternativ](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="a9cc0-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="a9cc0-109">Pentru a rezolva aceste probleme, a se vedea [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="a9cc0-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="a9cc0-110">În cazul în care problemele anterioare nu se aplică, executaţi raportul regulă Inbox de diagnosticare înainte să escaladeze emiterii către Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="a9cc0-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="a9cc0-111">Deschide cutia poştală în Outlook pe web, şi faceţi clic pe **Setări** \> **Opţiuni** \> **Organize e-mail** \> **regulile pentru Inbox**.</span><span class="sxs-lookup"><span data-stu-id="a9cc0-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="a9cc0-112">În partea de jos a paginii, faceţi clic pe **dacă regulile tale nu sunt de lucru faceţi clic aici pentru a genera un raport de diagnostic**.</span><span class="sxs-lookup"><span data-stu-id="a9cc0-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
