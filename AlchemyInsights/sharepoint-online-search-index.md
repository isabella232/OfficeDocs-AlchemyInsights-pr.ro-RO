---
title: Căutare în SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507643"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="d5e46-102">Accesarea cu crawlere conţinut şi indexarea în SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d5e46-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="d5e46-103">Conţinutul trebuie să fie indexat şi adăugate la indexul de căutare pentru utilizatorilor să găsească ceea ce ei caută în SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="d5e46-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="d5e46-104">Conţinutul este scotocit automat bazat pe un program de accesare cu crawlere pre-definite (programul de scotocire nu poate fi schimbat).</span><span class="sxs-lookup"><span data-stu-id="d5e46-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="d5e46-105">Crawler-ul preia conţinutul pe care s-a schimbat ultima scotocire şi actualizează indexul.</span><span class="sxs-lookup"><span data-stu-id="d5e46-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="d5e46-106">Pentru a se asigura de conţinut este indexat şi Indexul este actualizat, reţineţi următoarele:</span><span class="sxs-lookup"><span data-stu-id="d5e46-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="d5e46-107">Asiguraţi-vă că de conţinut pot fi găsite făcând [conţinutul site-ului poate fi căutat](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="d5e46-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="d5e46-108">Aţi modificat o proprietate gestionată, sau atunci când aţi schimbat cartografierea accesate şi gestionate proprietăţi, site-ul trebuie să fie re-scotocite înainte de modificările vor fi reflectate în indexul de căutare.</span><span class="sxs-lookup"><span data-stu-id="d5e46-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="d5e46-109">Deoarece modificările sunt făcute în schemă de căutare, şi nu la site-ul real, crawlerul va automat re-indexa site-ul.</span><span class="sxs-lookup"><span data-stu-id="d5e46-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="d5e46-110">Pentru mai multe informaţii, consultaţi [manual solicita accesarea cu crawlere şi re-indexarea unui site, o listă sau o bibliotecă](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="d5e46-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="d5e46-111">Aşteptaţi cel puţin 24 de ore după manual solicită o accesare cu crawlere şi complet re-index pentru a vedea dacă vă confruntaţi în continuare o problemă.</span><span class="sxs-lookup"><span data-stu-id="d5e46-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="d5e46-112">În cazul în care mai mult de 24 de ore au trecut de cand ai initiat de accesare cu crawlere şi complet re-indexa, vă rugăm să vă un caz de suport.</span><span class="sxs-lookup"><span data-stu-id="d5e46-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="d5e46-113">În multe cazuri, lucrăm deja la o soluţie.</span><span class="sxs-lookup"><span data-stu-id="d5e46-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="d5e46-114">Vă rugăm să ne dea cel puţin 24 de ore pentru a finaliza o soluţie.</span><span class="sxs-lookup"><span data-stu-id="d5e46-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d5e46-115">În cazul în care un site, documentul (biblioteca), sau o listă a fost şters şi prezintă încă în rezultatele de căutare, utilizatorii ar trebui să primiţi o **Eroare 404 Fişier negăsit** atunci când încearcă să-l acces.</span><span class="sxs-lookup"><span data-stu-id="d5e46-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="d5e46-116">Această problemă trebuie să fiţi conectat ca un caz de suport pentru o analiza ulterioara.</span><span class="sxs-lookup"><span data-stu-id="d5e46-116">This issue should be logged as a support case for further investigation.</span></span> 



