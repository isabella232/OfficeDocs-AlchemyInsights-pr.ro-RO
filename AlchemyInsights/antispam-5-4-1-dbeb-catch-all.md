---
title: AntiSpam 5.4.1 DBEB Catch-toate
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964277"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="4c1b6-102">Remedierea problemelor de livrare pentru codul de eroare 550 5.4.1 Releu acces refuzat</span><span class="sxs-lookup"><span data-stu-id="4c1b6-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="4c1b6-103">Această problemă apare atunci când [Verificați pentru a vedea dacă o adresă de e-mail este validă pentru a preveni bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) atunci când intră în rețeaua Office 365.</span><span class="sxs-lookup"><span data-stu-id="4c1b6-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="4c1b6-104">Încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="4c1b6-104">Try the following:</span></span>

1. <span data-ttu-id="4c1b6-105">Determinați dacă problema este specifică unui domeniu întreg sau unei singure adrese de e-mail:</span><span class="sxs-lookup"><span data-stu-id="4c1b6-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="4c1b6-106">Domeniu întreg: uneori, domeniul trebuie să fie sincronizat; Încercați [să setarea domeniului la interne și apoi înapoi la Authoritar](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="4c1b6-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
     - <span data-ttu-id="4c1b6-107">Singură adresă de e-mail: uneori, adresa trebuie să fie sincronizate; schimbarea adresei proxy SMTP și apoi schimbarea înapoi poate ajuta.</span><span class="sxs-lookup"><span data-stu-id="4c1b6-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="4c1b6-108">Determinați dacă problema este specifică unui grup sau unui folder public.</span><span class="sxs-lookup"><span data-stu-id="4c1b6-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="4c1b6-109">Pentru unele tipuri de obiecte, obiectele pot fi necesare pentru a fi create manual în Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4c1b6-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="4c1b6-110">Dacă aveți nevoie de ajutor suplimentar, vă rugăm să deschideți un bilet de suport și să specificați domeniul de aplicare al problemei (includidng tipul de obiect pe care îl trimiteți), astfel încât să vă putem asista mai bine.</span><span class="sxs-lookup"><span data-stu-id="4c1b6-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>