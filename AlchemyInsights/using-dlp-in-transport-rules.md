---
title: Utilizarea DLP în regulile de transport
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
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827228"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="f09cc-102">Utilizarea DLP în regulile de transport</span><span class="sxs-lookup"><span data-stu-id="f09cc-102">Using DLP in transport rules</span></span>

<span data-ttu-id="f09cc-103">Pentru a integra Prevenirea pierderii datelor (DLP) într-un transport existent, utilizați condiția „**Dacă mesajul conține... Informații confidențiale**” din setarea Regulă de transport.</span><span class="sxs-lookup"><span data-stu-id="f09cc-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="f09cc-104">**Pentru mai multe detalii, consultați:**</span><span class="sxs-lookup"><span data-stu-id="f09cc-104">**For more details, see:**</span></span>

- <span data-ttu-id="f09cc-105">Tipuri de informații confidențiale DLP integrate în regulile de transport: [Integrarea regulilor pentru informații confidențiale](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="f09cc-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="f09cc-106">De asemenea, puteți testa regula cu sau fără testarea politicii, utilizând Modul de testare din regulă.</span><span class="sxs-lookup"><span data-stu-id="f09cc-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="f09cc-107">Înainte de a testa o regulă, ar trebui să așteptați 30 de minute după crearea acesteia.</span><span class="sxs-lookup"><span data-stu-id="f09cc-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="f09cc-108">Consultați [Testați fluxul de corespondență/Reguli de transport](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="f09cc-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="f09cc-109">**Notă**: dacă încercați să implementați o politică DLP nouă cu regulile de transport în EAC, utilizați în schimb [Politicile DLP din Centrul de securitate și conformitate](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="f09cc-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
