---
title: fel ca filename este cel mai bun
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
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/25/2019
ms.locfileid: "35800057"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="1864d-102">Necesar header Alchemy H1, H2's nu funcționează.</span><span class="sxs-lookup"><span data-stu-id="1864d-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="1864d-103">Cele mai bune practici și orientări pentru Authoring Alchemy:</span><span class="sxs-lookup"><span data-stu-id="1864d-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="1864d-104">Nu **cuib Alchemy Insights în dosare**-acest lucru va rupe structura URL-ul.</span><span class="sxs-lookup"><span data-stu-id="1864d-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="1864d-105">Încercăm să reparăm asta.</span><span class="sxs-lookup"><span data-stu-id="1864d-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="1864d-106">Fișierele din folderul **Alchemyinsights** ar trebui să aibă nume de fișiere minuscule cu cratime pentru spațiile ex.</span><span class="sxs-lookup"><span data-stu-id="1864d-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="1864d-107">***să-Enable-litigiu-Hold***.</span><span class="sxs-lookup"><span data-stu-id="1864d-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="1864d-108">Includeți ID-ul de regulă sau ID-ul Cupei din [portalul de parteneri alchimie](https://alchemyportal.azurewebsites.net) în câmpul MS. Custom.</span><span class="sxs-lookup"><span data-stu-id="1864d-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="1864d-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="1864d-109">ex.</span></span> <span data-ttu-id="1864d-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="1864d-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="1864d-111">Utilizați restul metadatelor din partea de sus a acestui fișier ca șablon.</span><span class="sxs-lookup"><span data-stu-id="1864d-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="1864d-112">În [portalul pentru parteneri alchimie](https://alchemyportal.azurewebsites.net), navigați în jos la secțiunea **client Insight title:** și utilizați-o ca punct de plecare pentru titlul H1 pentru înțelegere.</span><span class="sxs-lookup"><span data-stu-id="1864d-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="1864d-113">Alchemy Insights trebuie să aibă doar un singur H1 în partea de sus sau vor sparge în producție.</span><span class="sxs-lookup"><span data-stu-id="1864d-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="1864d-114">H2s nu face nici atât utilizarea **Bold** sau alte convenții pentru a semnifica secțiuni separate.</span><span class="sxs-lookup"><span data-stu-id="1864d-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="1864d-115">Apoi, completați textul corpului utilizând proiectul de material din secțiunea statistici client din pagina de regulă alchimie</span><span class="sxs-lookup"><span data-stu-id="1864d-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="1864d-116">Listele cu marcatori sunt bune</span><span class="sxs-lookup"><span data-stu-id="1864d-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="1864d-117">Liste numerotate prea</span><span class="sxs-lookup"><span data-stu-id="1864d-117">Numbered lists too</span></span>
    1. <span data-ttu-id="1864d-118">**Bold** și *cursiv* sunt un-OK</span><span class="sxs-lookup"><span data-stu-id="1864d-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="1864d-119">Link-uri ar trebui să fie întotdeauna fie **"link-uri către web"/externe** sau **Deep-link-uri către elemente UI**, nu link-uri interne.</span><span class="sxs-lookup"><span data-stu-id="1864d-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="1864d-120">Imaginile nu sunt acceptate oficial în acest moment, dar este pe foaia de parcurs.</span><span class="sxs-lookup"><span data-stu-id="1864d-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="1864d-121">Și acest lucru este într-adevăr deja un pic prea mult timp.</span><span class="sxs-lookup"><span data-stu-id="1864d-121">And this is really already a bit too long.</span></span> <span data-ttu-id="1864d-122">Cele mai bune practici este de aproximativ 400 de caractere---------------------------------</span><span class="sxs-lookup"><span data-stu-id="1864d-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="1864d-123">După ce conținutul este gata, trageți-l în ramura live.</span><span class="sxs-lookup"><span data-stu-id="1864d-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="1864d-124">Apoi, mergeți la [portalul de parteneri alchimie](https://alchemyportal.azurewebsites.net) și introduceți numele fișierului în câmpul URL.</span><span class="sxs-lookup"><span data-stu-id="1864d-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 