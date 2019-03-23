---
title: 1491-Search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776093"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="a8981-102">Căutare conţinutul nu returna rezultatele aşteptate</span><span class="sxs-lookup"><span data-stu-id="a8981-102">Content Search not returning expected results</span></span>

<span data-ttu-id="a8981-103">Atunci când rulează conţinut căutări din Office 365 securitate & centru de conformitate, puteţi primi rezultate neaşteptate.</span><span class="sxs-lookup"><span data-stu-id="a8981-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="a8981-104">Luaţi în considerare următoarele lucruri care pot afecta rezultatele căutării:</span><span class="sxs-lookup"><span data-stu-id="a8981-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="a8981-105">**Locaţii de conţinut şi condiţiile de căutare**: Asiguraţi-vă că aţi selectat locatiile conţinut adecvat şi condiţii de căutare.</span><span class="sxs-lookup"><span data-stu-id="a8981-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="a8981-106">Dacă aţi rulat o căutaţi mare (cu mai multe locaţii), ia în considerare o diviza în mai multe căutări.</span><span class="sxs-lookup"><span data-stu-id="a8981-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="a8981-107">**Parţial indexat articole**: [parţial indexate elementele](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) din cutiile poştale sunt incluse în rezultatele de căutare estimată.</span><span class="sxs-lookup"><span data-stu-id="a8981-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="a8981-108">Cu toate acestea, parţial indexate elemente din site-urile SharePoint și OneDrive nu sunt incluse în estimarea de căutare.</span><span class="sxs-lookup"><span data-stu-id="a8981-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="a8981-109">**Eşecuri de căutare**: atunci când caută un număr mare de cutii poştale (peste 100.000 poştale), este posibil să primiţi erori de căutare, cu codurile de eroare, cum ar fi CS008-009 si CS012-002).</span><span class="sxs-lookup"><span data-stu-id="a8981-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="a8981-110">În acest caz, încercaţi din nou căutare doar pentru locatii de conţinut nu a reuşit.</span><span class="sxs-lookup"><span data-stu-id="a8981-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="a8981-111">A se vedea [acest articol](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) pentru mai multe informaţii.</span><span class="sxs-lookup"><span data-stu-id="a8981-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
