---
title: Conținutul nu apare în rezultatele căutării SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705673"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="9c4e3-102">Conținutul nu apare în rezultatele căutării SharePoint</span><span class="sxs-lookup"><span data-stu-id="9c4e3-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="9c4e3-103">Urmați acești pași de depanare atunci când conținutul așteptat nu apare în rezultatele căutării:</span><span class="sxs-lookup"><span data-stu-id="9c4e3-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="9c4e3-104">Verificați dacă **site-ul** care conține conținutul așteptat este setat pentru a permite conținutului să apară în rezultatele căutării.</span><span class="sxs-lookup"><span data-stu-id="9c4e3-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="9c4e3-105">Urmați pașii din [Afișare conținut pe un site în rezultatele căutării](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="9c4e3-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="9c4e3-106">Verificați dacă **lista** sau **biblioteca** care conține conținutul așteptat este setată pentru a permite conținutul să apară în rezultatele căutării.</span><span class="sxs-lookup"><span data-stu-id="9c4e3-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="9c4e3-107">Urmați pașii [din Afișare conținut din liste sau biblioteci în rezultatele căutării](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="9c4e3-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="9c4e3-108">Verificați dacă pagina, documentul sau aspectul particularizat al paginii sunt publicate ca **versiune majoră.**</span><span class="sxs-lookup"><span data-stu-id="9c4e3-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="9c4e3-109">Urmați pasul 3 în [Căutare nu returnează toate rezultatele în SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="9c4e3-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="9c4e3-110">Verificați dacă utilizatorul are **permisiuni pentru** a vizualiza conținutul.</span><span class="sxs-lookup"><span data-stu-id="9c4e3-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="9c4e3-111">Urmați pașii din [Înțelegerea nivelurilor de permisiune din SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="9c4e3-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="9c4e3-112">Dacă schema de căutare a fost modificată prin adăugarea unei proprietăți gestionate noi, prin editarea unei proprietăți gestionate sau prin eliminarea unei proprietăți gestionate, atunci va fi necesară o scotocire și un reindex.</span><span class="sxs-lookup"><span data-stu-id="9c4e3-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="9c4e3-113">**Reindexați** conținutul urmând pașii din [Solicitarea manuală de scotocire și reindexare a unui site, a unei biblioteci sau a unei liste](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="9c4e3-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="9c4e3-114">Acest lucru poate dura un timp, așteptați 24 de ore înainte de a verifica rezultatele din nou.</span><span class="sxs-lookup"><span data-stu-id="9c4e3-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="9c4e3-115">Pentru mai multe informații, consultați [Activarea conținutului de pe un site pentru a putea fi căutat](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="9c4e3-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
