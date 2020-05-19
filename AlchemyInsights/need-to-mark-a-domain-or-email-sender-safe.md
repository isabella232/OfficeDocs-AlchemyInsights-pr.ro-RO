---
title: Trebuie să marcați un domeniu sau un expeditor de e-mail în siguranță?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281183"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="e049a-102">Trebuie să marcați un domeniu sau un expeditor de e-mail în siguranță?</span><span class="sxs-lookup"><span data-stu-id="e049a-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="e049a-103">Utilizarea listelor de **expeditori siguri nu este recomandată,** deoarece deschide organizația la atacuri spam, phish și falsificare.</span><span class="sxs-lookup"><span data-stu-id="e049a-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="e049a-104">Cu toate acestea, dacă există o cerință de afaceri, **vă recomandăm să** utilizați **[Reguli flux de corespondență](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pentru acest lucru.</span><span class="sxs-lookup"><span data-stu-id="e049a-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="e049a-105">Ghidul nostru asigură autentificarea expeditorului (verifică trimiterea domeniului nu este falsificată).</span><span class="sxs-lookup"><span data-stu-id="e049a-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="e049a-106">**Notă:** Nu recomandăm gestionarea informațiilor fals pozitive utilizând liste de expeditori siguri, deoarece excepțiile de la filtrarea spamului vă pot deschide organizația la atacuri de securitate.</span><span class="sxs-lookup"><span data-stu-id="e049a-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="e049a-107">Dacă utilizatorul (utilizatorii) primesc mesaje marcate incorect ca spam sau e-mail nedorit, **[raportați mesaje și fișiere la Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="e049a-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="e049a-108">Expeditorii siguri din Outlook, lista de expeditori permise sau lista de domenii permisă în politicile anti-spam **trebuie evitate,** deoarece expeditorii ocolesc toate mesajele spam, lingură și protecția phish și autentificarea expeditorului (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="e049a-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="e049a-109">Această metodă este cel mai bine utilizată numai pentru testarea temporară.</span><span class="sxs-lookup"><span data-stu-id="e049a-109">This method is best used for temporary testing only.</span></span>
