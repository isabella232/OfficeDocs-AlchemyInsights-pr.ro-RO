---
title: Instrumentul de export pentru descoperirea informațiilor electronic
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814600"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="ed8e3-102">Nu puteți să instalați sau să rulați Instrumentul de export pentru descoperirea informațiilor electronic?</span><span class="sxs-lookup"><span data-stu-id="ed8e3-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="ed8e3-103">Dacă nu puteți instala sau rula Instrumentul de export pentru descoperirea informațiilor electronic pentru a descărca rezultatele căutării, verificați următoarele:</span><span class="sxs-lookup"><span data-stu-id="ed8e3-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="ed8e3-104">Computerul pe care îl utilizați îndeplinește aceste cerințe predefinite:</span><span class="sxs-lookup"><span data-stu-id="ed8e3-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="ed8e3-105">Versiuni pe 32 sau pe 64 de biți de Windows 7 și versiuni mai recente</span><span class="sxs-lookup"><span data-stu-id="ed8e3-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="ed8e3-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="ed8e3-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="ed8e3-107">Un browser acceptat:</span><span class="sxs-lookup"><span data-stu-id="ed8e3-107">A supported browser:</span></span>

  - <span data-ttu-id="ed8e3-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="ed8e3-108">Microsoft Edge</span></span>

    <span data-ttu-id="ed8e3-109">Sau</span><span class="sxs-lookup"><span data-stu-id="ed8e3-109">Or</span></span>

  - <span data-ttu-id="ed8e3-110">Internet Explorer 10 și versiuni mai recente</span><span class="sxs-lookup"><span data-stu-id="ed8e3-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="ed8e3-111">Alte browsere, cum ar fi Google Chrome și Mozilla Firefox nu sunt acceptate.</span><span class="sxs-lookup"><span data-stu-id="ed8e3-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="ed8e3-112">Organizația dvs. se poate conecta la punctul final în Azure, care este **\* .blob.core.windows.net** (wildcardul reprezintă un identificator unic pentru munca dvs. de export).</span><span class="sxs-lookup"><span data-stu-id="ed8e3-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="ed8e3-113">În Centrul de conformitate de securitate Microsoft 365, i s-a atribuit rolul &amp; Export.</span><span class="sxs-lookup"><span data-stu-id="ed8e3-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="ed8e3-114">În mod implicit, acest rol este atribuit doar grupului de roluri Manager pentru descoperirea informațiilor electronic.</span><span class="sxs-lookup"><span data-stu-id="ed8e3-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="ed8e3-115">Consultați [Atribuirea permisiunilor de descoperire a informațiilor electronic.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="ed8e3-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="ed8e3-116">Pentru mai multe informații, consultați [Exportul rezultatelor căutării de conținut.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="ed8e3-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="ed8e3-117">Dacă exportați mai mult de 100.000 de cutii poștale, va trebui să utilizați următorul Powershell pentru a descărca rezultatele exportului: exportul rezultatelor din peste  [100.000](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)de cutii poștale.</span><span class="sxs-lookup"><span data-stu-id="ed8e3-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>