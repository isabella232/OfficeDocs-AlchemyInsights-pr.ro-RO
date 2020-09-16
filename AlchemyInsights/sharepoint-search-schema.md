---
title: Gestionarea schemei de căutare în SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770563"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="27685-102">Gestionarea schemei de căutare în SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="27685-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="27685-103">Schema de căutare controlează ce pot căuta utilizatorii, cum îl pot căuta utilizatorii și cum puteți prezenta rezultatele pe site-urile web de căutare.</span><span class="sxs-lookup"><span data-stu-id="27685-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="27685-104">Consultați [gestionarea schemei de căutare în SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) pentru a afla cum să:</span><span class="sxs-lookup"><span data-stu-id="27685-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="27685-105">Modificați schema de căutare.</span><span class="sxs-lookup"><span data-stu-id="27685-105">Change the search schema.</span></span>
- <span data-ttu-id="27685-106">Creați proprietăți gestionate.</span><span class="sxs-lookup"><span data-stu-id="27685-106">Create managed properties.</span></span>
- <span data-ttu-id="27685-107">Maparea hărților accesate cu crawlere la proprietățile gestionate.</span><span class="sxs-lookup"><span data-stu-id="27685-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="27685-108">Rețineți următoarele aspecte în ceea ce privește gestionarea schemei de căutare:</span><span class="sxs-lookup"><span data-stu-id="27685-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="27685-109">Dacă primiți un avertisment care indică **faptul că aplicația este întreruptă** atunci când faceți o modificare de schemă, aceasta este doar temporară, deoarece se produce întreținerea serviciului.</span><span class="sxs-lookup"><span data-stu-id="27685-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="27685-110">Dacă au trecut mai mult de 24 de ore și încă vă confruntați cu avertizarea, vă rugăm să înregistrați un caz de asistență.</span><span class="sxs-lookup"><span data-stu-id="27685-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="27685-111">Atunci când modificați proprietățile gestionate sau adăugați altele noi, modificările intră în vigoare numai după ce conținutul a fost reintrodus.</span><span class="sxs-lookup"><span data-stu-id="27685-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="27685-112">În SharePoint Online, accesarea cu crawlere se întâmplă automat în funcție de programul de accesare cu crawlere definit.</span><span class="sxs-lookup"><span data-stu-id="27685-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="27685-113">Pentru a vă asigura că modificările sunt accesate cu crawlere, puteți [solicita în mod specific reindexarea listei sau a bibliotecii](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="27685-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="27685-114">Pentru o prezentare generală completă a schemei de căutare, consultați [introducerea schemei de căutare](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="27685-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


