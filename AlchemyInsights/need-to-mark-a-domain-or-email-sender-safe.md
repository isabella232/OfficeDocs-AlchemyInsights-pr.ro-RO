---
title: Trebuie să marcați un domeniu sau un expeditor de e-mail ca sigur?
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
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792144"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="2c2f4-102">Trebuie să marcați un domeniu sau un expeditor de e-mail ca sigur?</span><span class="sxs-lookup"><span data-stu-id="2c2f4-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="2c2f4-103">Utilizarea **listelor de expeditori siguri** nu este recomandată, deoarece deschide organizația dvs. în atacuri de spam, fals și fals fals.</span><span class="sxs-lookup"><span data-stu-id="2c2f4-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="2c2f4-104">Cu toate acestea, dacă există o cerință de afaceri, vă **recomandăm să utilizați** reguli de flux de **[corespondență](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pentru acest lucru.</span><span class="sxs-lookup"><span data-stu-id="2c2f4-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="2c2f4-105">Instrucțiunile noastre asigură autentificarea expeditorului (verificarea domeniului de trimitere nu este falsificată).</span><span class="sxs-lookup"><span data-stu-id="2c2f4-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="2c2f4-106">**Notă:** Nu recomandăm gestionarea fals pozitive utilizând listele de expeditori siguri, deoarece excepțiile de la filtrarea antispam pot deschide organizația dvs. la atacuri de securitate.</span><span class="sxs-lookup"><span data-stu-id="2c2f4-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="2c2f4-107">Dacă utilizatorii dvs. primesc mesaje marcate incorect ca spam sau e-mailuri nedorite, **[raportați mesajele și fișierele la Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="2c2f4-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="2c2f4-108">Expeditorii siguri din Outlook, lista de expeditori blocați  sau lista de domenii permise din politicile antispam trebuie evitate, deoarece expeditorii ocolesc tot spamul, falsoful și protecția antispam și autentificarea expeditorului (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="2c2f4-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="2c2f4-109">Această metodă se utilizează cel mai bine numai pentru testarea temporară.</span><span class="sxs-lookup"><span data-stu-id="2c2f4-109">This method is best used for temporary testing only.</span></span>
