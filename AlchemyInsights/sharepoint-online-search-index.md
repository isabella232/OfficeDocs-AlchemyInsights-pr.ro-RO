---
title: Căutare în SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044055"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="411dc-102">Conținut scotocire și indexare în SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="411dc-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="411dc-103">Conținutul trebuie scotocit și adăugat la indexul de căutare pentru ca utilizatorii să găsească ceea ce caută în SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="411dc-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="411dc-104">Conținutul este scotocit automat pe baza unui program de scotocire predefinit (programul de scotocire nu poate fi modificat).</span><span class="sxs-lookup"><span data-stu-id="411dc-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="411dc-105">Crawlerul preia conținut care s-a modificat de la ultima accesare cu crawlere și actualizează indexul.</span><span class="sxs-lookup"><span data-stu-id="411dc-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="411dc-106">Pentru a asigura că conținutul este scotocit și indexul este actualizat, rețineți următoarele:</span><span class="sxs-lookup"><span data-stu-id="411dc-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="411dc-107">Asigurați-vă că conținutul poate fi găsit prin [crearea de conținut site-ul de căutare](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="411dc-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="411dc-108">Când ați modificat o proprietate gestionată sau când ați modificat Maparea proprietăților scotocite și gestionate, situl trebuie rescotocit înainte ca modificările să se reflecte în indexul de căutare.</span><span class="sxs-lookup"><span data-stu-id="411dc-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="411dc-109">Deoarece modificările sunt făcute în schema de căutare, și nu la site-ul real, crawlerul nu va reindexa automat site-ul.</span><span class="sxs-lookup"><span data-stu-id="411dc-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="411dc-110">Pentru mai multe informații, consultați [solicitați manual accesarea cu crawlere și reindexarea unui site, a unei biblioteci sau a unei liste](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="411dc-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="411dc-111">Așteptați cel puțin 24 de ore după ce solicitați manual o accesare cu crawlere și o Reindexare completă pentru a vedea dacă întâmpinați încă o problemă.</span><span class="sxs-lookup"><span data-stu-id="411dc-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="411dc-112">Dacă au trecut mai mult de 24 de ore de la inițierea scotocire și reindex complet, vă rugăm să faceți log un caz de suport.</span><span class="sxs-lookup"><span data-stu-id="411dc-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="411dc-113">În multe cazuri, suntem deja de lucru pe o soluție.</span><span class="sxs-lookup"><span data-stu-id="411dc-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="411dc-114">Vă rugăm să ne acordați cel puțin 24 de ore pentru a finaliza o soluție.</span><span class="sxs-lookup"><span data-stu-id="411dc-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="411dc-115">Dacă un site, document (bibliotecă), sau o listă a fost șters și încă arată în rezultatele căutării, utilizatorii ar trebui să primească o **eroare 404 fișier negăsit** atunci când încearcă să-l acceseze.</span><span class="sxs-lookup"><span data-stu-id="411dc-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="411dc-116">Această problemă ar trebui să fie înregistrată ca un caz de sprijin pentru investigații suplimentare.</span><span class="sxs-lookup"><span data-stu-id="411dc-116">This issue should be logged as a support case for further investigation.</span></span> 



