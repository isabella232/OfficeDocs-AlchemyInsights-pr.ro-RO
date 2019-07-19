---
title: fel de nume de fişier este cel mai bun
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b77e514da36701808d46248e8f2a45137751a1c7
ms.sourcegitcommit: 5447031f9d0a320c49897b8adb5d29ac9437fbc5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/18/2019
ms.locfileid: "35786425"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="5648d-102">Necesare alchimie antet H1, H2 pe nu funcţionează.</span><span class="sxs-lookup"><span data-stu-id="5648d-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="5648d-103">Cele mai bune practici și liniile directoare pentru authoring de Alchemy:</span><span class="sxs-lookup"><span data-stu-id="5648d-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="5648d-104">**Cuib alchimie intuiţii în dosare**- acest lucru va rupe structura de URL-ul.</span><span class="sxs-lookup"><span data-stu-id="5648d-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="5648d-105">Suntem în căutarea în stabilirea acest lucru.</span><span class="sxs-lookup"><span data-stu-id="5648d-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="5648d-106">Fişierele din folderul **AlchemyInsights** trebuie să aibă minuscule de fişiere cu cratime pentru spaţiile ex.</span><span class="sxs-lookup"><span data-stu-id="5648d-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="5648d-107">***Cum-la spre-enable--litigiu***.</span><span class="sxs-lookup"><span data-stu-id="5648d-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="5648d-108">Includ ID regula ID sau găleată din [alchimie partener portal](https://alchemyportal.azurewebsites.net) în domeniul ms.custom.</span><span class="sxs-lookup"><span data-stu-id="5648d-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="5648d-109">ex.</span><span class="sxs-lookup"><span data-stu-id="5648d-109">ex.</span></span> <span data-ttu-id="5648d-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="5648d-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="5648d-111">Utilizaţi restul de metadate în partea de sus a acestui fișier ca șablon.</span><span class="sxs-lookup"><span data-stu-id="5648d-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="5648d-112">În [alchimie partener portal](https://alchemyportal.azurewebsites.net), navigaţi în jos la secţiunea **titlu de carte de vizita clientului:** și care, ca începând cu un punct pentru H1 titlu pentru înţelegere.</span><span class="sxs-lookup"><span data-stu-id="5648d-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="5648d-113">Alchimia intuiţii trebuie să aibă doar un singur H1 la partea de sus sau se va intrerupe în producţie.</span><span class="sxs-lookup"><span data-stu-id="5648d-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="5648d-114">H2s nu face atât utilizarea **îndrăzneţ** sau alte convenții înseamnă secţiuni separate.</span><span class="sxs-lookup"><span data-stu-id="5648d-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="5648d-115">Apoi, completaţi în corpul textului folosind materiale de proiect în secţiunea clientului intuiţii a paginii de regulă de alchimie</span><span class="sxs-lookup"><span data-stu-id="5648d-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="5648d-116">Liste cu marcatori sunt bine</span><span class="sxs-lookup"><span data-stu-id="5648d-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="5648d-117">Liste numerotate prea</span><span class="sxs-lookup"><span data-stu-id="5648d-117">Numbered lists too</span></span>
    1. <span data-ttu-id="5648d-118">**Bold** şi *cursive* sunt un-OK</span><span class="sxs-lookup"><span data-stu-id="5648d-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="5648d-119">Link-uri ar trebui să fie întotdeauna **"link-uri la web" / extern** OR **adânc-link-uri la elemente de UI**, link-uri nu interne.</span><span class="sxs-lookup"><span data-stu-id="5648d-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="5648d-120">Imaginile nu sunt suportate oficial în acest moment, dar este pe foaia de parcurs.</span><span class="sxs-lookup"><span data-stu-id="5648d-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="5648d-121">Şi acest lucru este într-adevăr deja un pic prea lung.</span><span class="sxs-lookup"><span data-stu-id="5648d-121">And this is really already a bit too long.</span></span> <span data-ttu-id="5648d-122">Cele mai bune practici este de aproximativ 400 de caractere---</span><span class="sxs-lookup"><span data-stu-id="5648d-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="5648d-123">Odată ce conţinutul este gata, trageţi-l la sucursala live.</span><span class="sxs-lookup"><span data-stu-id="5648d-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="5648d-124">Apoi, du-te la [portalului Partner de alchimie](https://alchemyportal.azurewebsites.net) şi introduceţi numele fişierului în câmpul URL-ul.</span><span class="sxs-lookup"><span data-stu-id="5648d-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 


