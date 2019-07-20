---
title: Conţinut fără rezultate
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800538"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="ae97b-102">Nici un rezultat la conţinut căutare/exporturilor</span><span class="sxs-lookup"><span data-stu-id="ae97b-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="ae97b-103">Probleme cu conţinut căutare/exporturile nu reveni orice date se poate datora anumitor filtru de securitate a conformității care a fost de configurare de un Admin specifice şi nu se comunică la toate administratori.</span><span class="sxs-lookup"><span data-stu-id="ae97b-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="ae97b-104">Pentru a rezolva acest lucru, verificaţi pentru a vedea dacă există orice conformitatea filtrele de securitate care poate fi cauza acest lucru:</span><span class="sxs-lookup"><span data-stu-id="ae97b-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="ae97b-105">Conecta la securitatea şi conformitatea centrul Powershell</span><span class="sxs-lookup"><span data-stu-id="ae97b-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="ae97b-106">Executaţi comenzile următoare:</span><span class="sxs-lookup"><span data-stu-id="ae97b-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="ae97b-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="ae97b-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="ae97b-108">Get-ComplianceSecurityFilter-organizare $org</span><span class="sxs-lookup"><span data-stu-id="ae97b-108">Get-ComplianceSecurityFilter -Organization $org</span></span>