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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516791"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="8b658-102">Nici un rezultat la conţinut căutare/exporturilor</span><span class="sxs-lookup"><span data-stu-id="8b658-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="8b658-103">Probleme cu conţinut căutare/exporturile nu reveni orice date se poate datora anumitor filtru de securitate a conformității care a fost de configurare de un Admin specifice şi nu se comunică la toate administratori.</span><span class="sxs-lookup"><span data-stu-id="8b658-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="8b658-104">Pentru a rezolva acest lucru, verificaţi pentru a vedea dacă există orice conformitatea filtrele de securitate care poate fi cauza acest lucru:</span><span class="sxs-lookup"><span data-stu-id="8b658-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="8b658-105">Conecta la securitatea şi conformitatea centrul Powershell</span><span class="sxs-lookup"><span data-stu-id="8b658-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="8b658-106">Executaţi comenzile următoare:</span><span class="sxs-lookup"><span data-stu-id="8b658-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="8b658-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="8b658-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="8b658-108">Get-ComplianceSecurityFilter-organizare $org</span><span class="sxs-lookup"><span data-stu-id="8b658-108">Get-ComplianceSecurityFilter -Organization $org</span></span>