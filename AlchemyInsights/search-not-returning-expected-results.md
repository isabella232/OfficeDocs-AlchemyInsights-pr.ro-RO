---
title: 1491-căutare-nu-returnare-așteptat-Rezultate
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740486"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="1558a-102">Căutarea de conținut nu returnează rezultatele așteptate</span><span class="sxs-lookup"><span data-stu-id="1558a-102">Content Search not returning expected results</span></span>

<span data-ttu-id="1558a-103">Atunci când se execută căutări de conținut din centrul de conformitate Microsoft 365 Security &, este posibil să primiți rezultate neașteptate de căutare.</span><span class="sxs-lookup"><span data-stu-id="1558a-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="1558a-104">Luați în considerare următoarele lucruri care vă pot afecta rezultatele căutării:</span><span class="sxs-lookup"><span data-stu-id="1558a-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="1558a-105">**Locații de conținut și condiții de căutare**: Asigurați-vă că ați selectat locațiile de conținut corespunzătoare și condițiile de căutare.</span><span class="sxs-lookup"><span data-stu-id="1558a-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="1558a-106">Dacă ați rulat o căutare mare (cu multe locații), luați în considerare împărțirea acesteia în mai multe căutări.</span><span class="sxs-lookup"><span data-stu-id="1558a-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="1558a-107">**Elemente indexate parțial**:  [elementele indexate parțial](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) din cutiile poștale sunt incluse în rezultatele de căutare estimate.</span><span class="sxs-lookup"><span data-stu-id="1558a-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="1558a-108">Cu toate acestea, elementele indexate parțial din site-uri în SharePoint și OneDrive nu sunt incluse în estimarea de căutare.</span><span class="sxs-lookup"><span data-stu-id="1558a-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="1558a-109">**Erori de căutare**: atunci când căutați un număr mare de cutii poștale (peste 100.000 de cutii poștale), este posibil să primiți erori de căutare, cu coduri de eroare, cum ar fi CS008-009 și CS012-002).</span><span class="sxs-lookup"><span data-stu-id="1558a-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="1558a-110">În acest caz, încercați din nou căutarea doar pentru locațiile de conținut nereușite.</span><span class="sxs-lookup"><span data-stu-id="1558a-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="1558a-111">Pentru mai multe informații, consultați  [acest articol](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="1558a-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
