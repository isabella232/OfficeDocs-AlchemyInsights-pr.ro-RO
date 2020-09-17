---
title: Doriți să marcați în siguranță un domeniu sau un expeditor de e-mail?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803257"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="b3558-102">Doriți să marcați în siguranță un domeniu sau un expeditor de e-mail?</span><span class="sxs-lookup"><span data-stu-id="b3558-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="b3558-103">Utilizarea **listelor de expeditori siguri nu este recomandată** , deoarece vă deschide organizația la atacuri spam, phishing și falsificare.</span><span class="sxs-lookup"><span data-stu-id="b3558-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="b3558-104">Cu toate acestea, dacă există o cerință de afaceri, vă **recomandăm** să utilizați **[regulile de flux de corespondență](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pentru aceasta.</span><span class="sxs-lookup"><span data-stu-id="b3558-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="b3558-105">Ghidul nostru asigură autentificarea expeditorului (verifică dacă trimiterea domeniului nu este falsificată).</span><span class="sxs-lookup"><span data-stu-id="b3558-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="b3558-106">**Notă**: nu recomandăm gestionarea unor valori false pozitive utilizând listele de expeditori siguri, deoarece excepțiile de la Filtrarea antispam pot deschide organizația la atacuri de securitate.</span><span class="sxs-lookup"><span data-stu-id="b3558-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="b3558-107">Dacă utilizatorii primesc mesaje marcate incorect ca spam sau e-mailuri nedorite, **[Raportați mesaje și fișiere la Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="b3558-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="b3558-108">Expeditorii siguri din Outlook, lista Expeditori acceptați sau lista de domenii permise în politicile anti-spam **trebuie evitate** , deoarece expeditorii ocolesc toate protecția antispam, spoof și phishing și autentificarea expeditorului (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="b3558-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="b3558-109">Această metodă este utilizată cel mai bine doar pentru testarea temporară.</span><span class="sxs-lookup"><span data-stu-id="b3558-109">This method is best used for temporary testing only.</span></span>
