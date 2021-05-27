---
title: Inventarul de software lipsește sau nu este corect
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676512"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="3d443-102">Inventarul de software lipsește sau nu este corect</span><span class="sxs-lookup"><span data-stu-id="3d443-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="3d443-103">Inventarul de software din Gestiunea amenințărilor și vulnerabilităților (TVM) este o listă de software cunoscut din organizația dvs., cu liste oficiale de enumerare a platformelor comune (CPE).</span><span class="sxs-lookup"><span data-stu-id="3d443-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="3d443-104">Produsele software fără o CPE oficială nu au vulnerabilități publicate.</span><span class="sxs-lookup"><span data-stu-id="3d443-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="3d443-105">Inventarul include, de asemenea, detalii precum numele furnizorului, numărul de amenințări, amenințările și numărul de dispozitive expuse.</span><span class="sxs-lookup"><span data-stu-id="3d443-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="3d443-106">Modificările de software de pe dispozitive se reflectă de obicei în portalurile de securitate în termen de două ore.</span><span class="sxs-lookup"><span data-stu-id="3d443-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="3d443-107">Totuși, uneori poate dura mai mult.</span><span class="sxs-lookup"><span data-stu-id="3d443-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="3d443-108">Momentan nu există nicio modalitate de a impune o sincronizare; este o evaluare continuă continuă.</span><span class="sxs-lookup"><span data-stu-id="3d443-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="3d443-109">Dacă faceți o modificare de software și modificarea nu se reflectă corect în TVM după 5 ore, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="3d443-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="3d443-110">Verificați secțiunea de dovezi software pentru a înțelege cum a fost detectat software-ul.</span><span class="sxs-lookup"><span data-stu-id="3d443-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="3d443-111">Asigurați-vă că software-ul este acceptat.</span><span class="sxs-lookup"><span data-stu-id="3d443-111">Make sure that the software is supported.</span></span> <span data-ttu-id="3d443-112">Software-ul poate fi vizibil doar la nivel de dispozitiv, chiar dacă în prezent nu este acceptat de Gestiunea amenințărilor și vulnerabilităților.</span><span class="sxs-lookup"><span data-stu-id="3d443-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="3d443-113">Cu toate acestea, sunt disponibile doar date limitate.</span><span class="sxs-lookup"><span data-stu-id="3d443-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="3d443-114">Pentru pașii necesari raportului inaccuracy din portal, consultați [Inaccuracy raport.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)</span><span class="sxs-lookup"><span data-stu-id="3d443-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="3d443-115">**Notă:** raportarea unei inadvertenări din portalul MDE este un canal uni-sens către inginerie.</span><span class="sxs-lookup"><span data-stu-id="3d443-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="3d443-116">Dacă problema este urgentă, deschideți un tichet de asistență.</span><span class="sxs-lookup"><span data-stu-id="3d443-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="3d443-117">Pentru mai multe informații, consultați [Inventar software - Gestiunea amenințărilor și vulnerabilităților](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="3d443-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>