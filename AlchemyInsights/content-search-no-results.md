---
title: Căutare conținut niciun rezultat
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680659"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="b57da-102">Niciun rezultat din căutarea de conținut/exporturi</span><span class="sxs-lookup"><span data-stu-id="b57da-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="b57da-103">Probleme cu căutarea de conținut/exporturile care nu returnează date pot fi cauzate de un anumit filtru de securitate de conformitate care a fost configurat de un anumit administrator și nu l-a comunicat tuturor administratorilor.</span><span class="sxs-lookup"><span data-stu-id="b57da-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="b57da-104">Pentru a rezolva acest lucru, Verificați dacă există filtre de securitate conformității care pot provoca acest lucru:</span><span class="sxs-lookup"><span data-stu-id="b57da-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="b57da-105">Conectarea la centrul de securitate și conformitate PowerShell</span><span class="sxs-lookup"><span data-stu-id="b57da-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="b57da-106">Rulează următorul commandlet:</span><span class="sxs-lookup"><span data-stu-id="b57da-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="b57da-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="b57da-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="b57da-108">Get-ComplianceSecurityFilter-organizație $org</span><span class="sxs-lookup"><span data-stu-id="b57da-108">Get-ComplianceSecurityFilter -Organization $org</span></span>