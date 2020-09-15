---
title: AntiSpam 5.4.1 DBEB captură-toate
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717373"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="1884b-102">Remedierea problemelor de livrare pentru codul de eroare 550 5.4.1 Releu Access Denied</span><span class="sxs-lookup"><span data-stu-id="1884b-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="1884b-103">Această problemă apare atunci când [Căutați pentru a vedea dacă o adresă de e-mail este validă pentru a împiedica bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) atunci când introduceți rețeaua Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1884b-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="1884b-104">Încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="1884b-104">Try the following:</span></span>

1. <span data-ttu-id="1884b-105">Determinați dacă problema este specifică pentru un domeniu întreg sau pentru o singură adresă de e-mail:</span><span class="sxs-lookup"><span data-stu-id="1884b-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="1884b-106">Domeniu întreg: uneori, domeniul trebuie sincronizat; Încercați să [Setați domeniul la intern, apoi înapoi la autoritate](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="1884b-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="1884b-107">Adresă de e-mail unică: uneori, adresa trebuie sincronizată; Modificarea adresei proxy SMTP, apoi modificarea sa înapoi vă poate ajuta.</span><span class="sxs-lookup"><span data-stu-id="1884b-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="1884b-108">Determinați dacă problema este specifică pentru un grup sau un folder public.</span><span class="sxs-lookup"><span data-stu-id="1884b-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="1884b-109">Pentru unele tipuri de obiecte, este posibil ca obiectele să trebuiască să fie create manual în Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1884b-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="1884b-110">Dacă aveți nevoie de ajutor suplimentar, vă rugăm să deschideți un tichet de asistență și să specificați domeniul problemei (inclusiv tipul de obiect pe care îl trimiteți) pentru a vă putea ajuta mai bine.</span><span class="sxs-lookup"><span data-stu-id="1884b-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>