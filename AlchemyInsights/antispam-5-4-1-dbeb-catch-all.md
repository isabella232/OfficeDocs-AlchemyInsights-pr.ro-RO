---
title: AntiSpam 5.4.1 DBEB catch-all AntiSpam 5.4.1 DBEB catch-all AntiSpam 5.4.1 DBEB catch-all AntiSpam
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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707923"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="f8e3e-102">Remedierea problemelor de livrare pentru codul de eroare 550 5.4.1 Releu de acces refuzat</span><span class="sxs-lookup"><span data-stu-id="f8e3e-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="f8e3e-103">Această problemă apare atunci când [verificați pentru a vedea dacă o adresă de poștă electronică este validă pentru a preveni bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) atunci când intră în rețeaua Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f8e3e-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="f8e3e-104">Încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="f8e3e-104">Try the following:</span></span>

1. <span data-ttu-id="f8e3e-105">Determinați dacă problema este specifică unui domeniu întreg sau unei singure adrese de e-mail:</span><span class="sxs-lookup"><span data-stu-id="f8e3e-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="f8e3e-106">Domeniu întreg: Uneori, domeniul trebuie sincronizat; încercați [să setezeți domeniul la intern și apoi înapoi la autoritate](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="f8e3e-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="f8e3e-107">Adresă de e-mail unică: Uneori, adresa trebuie sincronizată; schimbarea adresei proxy smtp și apoi schimbarea-l înapoi poate ajuta.</span><span class="sxs-lookup"><span data-stu-id="f8e3e-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="f8e3e-108">Determinați dacă problema este specifică unui grup sau unui folder public.</span><span class="sxs-lookup"><span data-stu-id="f8e3e-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="f8e3e-109">Pentru unele tipuri de obiecte, obiectele poate fi necesar să fie create manual în Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f8e3e-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="f8e3e-110">Dacă aveți nevoie de ajutor suplimentar, deschideți un bilet de asistență și specificați domeniul de aplicare al problemei (inclusiv tipul de obiect la care trimiteți), astfel încât să vă putem ajuta mai bine.</span><span class="sxs-lookup"><span data-stu-id="f8e3e-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>