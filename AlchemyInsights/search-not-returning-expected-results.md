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
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 094da9d75013aae56ca219b7ae03e85736ce5ee0
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551427"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="2c10f-102">Căutare conţinutul nu returna rezultatele aşteptate</span><span class="sxs-lookup"><span data-stu-id="2c10f-102">Content Search not returning expected results</span></span>

<span data-ttu-id="2c10f-103">Atunci când rulează conţinut căutări din Office 365 securitate & centru de conformitate, puteţi primi rezultate neaşteptate.</span><span class="sxs-lookup"><span data-stu-id="2c10f-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="2c10f-104">Luaţi în considerare următoarele lucruri care pot afecta rezultatele căutării:</span><span class="sxs-lookup"><span data-stu-id="2c10f-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="2c10f-105">**Locaţii de conţinut şi condiţiile de căutare**: Asiguraţi-vă că aţi selectat locatiile conţinut adecvat şi condiţii de căutare.</span><span class="sxs-lookup"><span data-stu-id="2c10f-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="2c10f-106">Dacă aţi rulat o căutaţi mare (cu mai multe locaţii), ia în considerare o diviza în mai multe căutări.</span><span class="sxs-lookup"><span data-stu-id="2c10f-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="2c10f-107">**Parţial indexat articole**: [parţial indexate elementele](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) din cutiile poştale sunt incluse în rezultatele de căutare estimată.</span><span class="sxs-lookup"><span data-stu-id="2c10f-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="2c10f-108">Cu toate acestea, parţial indexate elemente din site-urile SharePoint și OneDrive nu sunt incluse în estimarea de căutare.</span><span class="sxs-lookup"><span data-stu-id="2c10f-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="2c10f-109">**Eşecuri de căutare**: atunci când caută un număr mare de cutii poştale (peste 100.000 poştale), este posibil să primiţi erori de căutare, cu codurile de eroare, cum ar fi CS008-009 si CS012-002).</span><span class="sxs-lookup"><span data-stu-id="2c10f-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="2c10f-110">În acest caz, încercaţi din nou căutare doar pentru locatii de conţinut nu a reuşit.</span><span class="sxs-lookup"><span data-stu-id="2c10f-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="2c10f-111">A se vedea [acest articol](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) pentru mai multe informaţii.</span><span class="sxs-lookup"><span data-stu-id="2c10f-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
