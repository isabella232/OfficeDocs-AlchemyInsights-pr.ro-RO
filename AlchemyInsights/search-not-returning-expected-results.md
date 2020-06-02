---
title: 1491-căutare-nu-returnare-așteptat-rezultate
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510584"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="c83ea-102">Căutare conținut nu returnează rezultatele așteptate</span><span class="sxs-lookup"><span data-stu-id="c83ea-102">Content Search not returning expected results</span></span>

<span data-ttu-id="c83ea-103">Atunci când executați căutări de conținut din Centrul de securitate Microsoft 365 & conformitate, este posibil să primiți rezultate neașteptate de căutare.</span><span class="sxs-lookup"><span data-stu-id="c83ea-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="c83ea-104">Luați în considerare următoarele lucruri care pot afecta rezultatele căutării:</span><span class="sxs-lookup"><span data-stu-id="c83ea-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="c83ea-105">**Locații de conținut și condiții de căutare**: Asigurați-vă că ați selectat locațiile corespunzătoare ale conținutului și condițiile de căutare.</span><span class="sxs-lookup"><span data-stu-id="c83ea-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="c83ea-106">Dacă ați efectuat o căutare amplă (cu multe locații), luați în considerare împărțirea acesteia în mai multe căutări.</span><span class="sxs-lookup"><span data-stu-id="c83ea-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="c83ea-107">**Elemente parțial indexate:** [Elementele parțial indexate](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) din cutiile poștale sunt incluse în rezultatele căutării estimate.</span><span class="sxs-lookup"><span data-stu-id="c83ea-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="c83ea-108">Cu toate acestea, elementele parțial indexate de pe site-uri din SharePoint și OneDrive nu sunt incluse în estimarea de căutare.</span><span class="sxs-lookup"><span data-stu-id="c83ea-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="c83ea-109">**Erori de căutare**: Când căutați un număr mare de cutii poștale (peste 100.000 de cutii poștale), este posibil să obțineți erori de căutare, cu coduri de eroare, ar fi CS008-009 și CS012-002).</span><span class="sxs-lookup"><span data-stu-id="c83ea-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="c83ea-110">În acest caz, încercați din nou căutarea numai pentru locațiile de conținut nereușite.</span><span class="sxs-lookup"><span data-stu-id="c83ea-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="c83ea-111">Consultați [acest articol](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="c83ea-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
