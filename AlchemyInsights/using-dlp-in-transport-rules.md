---
title: Utilizarea DLP în regulile de transport
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915191"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="c2e76-102">Utilizarea DLP în regulile de transport</span><span class="sxs-lookup"><span data-stu-id="c2e76-102">Using DLP in transport rules</span></span>

<span data-ttu-id="c2e76-103">Pentru a integra Prevenirea pierderii datelor (DLP) într-un transport existent, utilizați condiția „**Dacă mesajul conține... Informații confidențiale**” din setarea Regulă de transport.</span><span class="sxs-lookup"><span data-stu-id="c2e76-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="c2e76-104">**Pentru mai multe detalii, consultați:**</span><span class="sxs-lookup"><span data-stu-id="c2e76-104">**For more details, see:**</span></span>

- <span data-ttu-id="c2e76-105">Tipuri de informații confidențiale DLP integrate în regulile de transport: [Integrarea regulilor pentru informații confidențiale](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="c2e76-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="c2e76-106">De asemenea, puteți testa regula cu sau fără testarea politicii, utilizând Modul de testare din regulă.</span><span class="sxs-lookup"><span data-stu-id="c2e76-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="c2e76-107">Înainte de a testa o regulă, ar trebui să așteptați 30 de minute după crearea acesteia.</span><span class="sxs-lookup"><span data-stu-id="c2e76-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="c2e76-108">Consultați [Testați fluxul de corespondență/Reguli de transport](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="c2e76-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="c2e76-109">**Notă**: dacă încercați să implementați o politică DLP nouă cu regulile de transport în EAC, utilizați în schimb [Politicile DLP din Centrul de securitate și conformitate](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="c2e76-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
