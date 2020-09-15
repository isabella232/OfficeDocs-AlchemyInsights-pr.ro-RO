---
title: la fel ca numele de fișier este cel mai bun
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664146"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="ba27c-102">"Antetul Alchemy necesar H1, H2 servește nu funcționează."</span><span class="sxs-lookup"><span data-stu-id="ba27c-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="ba27c-103">Cele mai bune practici și instrucțiuni pentru crearea Alchemy:</span><span class="sxs-lookup"><span data-stu-id="ba27c-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="ba27c-104">Nu **imbricați Insights Alchemy în foldere**-aceasta va întrerupe structura URL-ului.</span><span class="sxs-lookup"><span data-stu-id="ba27c-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="ba27c-105">Încercăm să reparăm asta.</span><span class="sxs-lookup"><span data-stu-id="ba27c-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="ba27c-106">Fișierele din folderul **AlchemyInsights** trebuie să aibă nume de fișiere minuscule cu cratime pentru spațiile ex.</span><span class="sxs-lookup"><span data-stu-id="ba27c-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="ba27c-107">***cum să activați-litigii-țineți***.</span><span class="sxs-lookup"><span data-stu-id="ba27c-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="ba27c-108">Includeți ID-ul de regulă sau ID-ul de cupă din [portalul partener Alchemy](https://alchemyportal.azurewebsites.net) în câmpul MS. Custom.</span><span class="sxs-lookup"><span data-stu-id="ba27c-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="ba27c-109">exemplu.</span><span class="sxs-lookup"><span data-stu-id="ba27c-109">ex.</span></span> <span data-ttu-id="ba27c-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="ba27c-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="ba27c-111">Utilizați restul metadatelor din partea de sus a acestui fișier ca șablon.</span><span class="sxs-lookup"><span data-stu-id="ba27c-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="ba27c-112">În [portalul partener Alchemy](https://alchemyportal.azurewebsites.net), navigați în jos la secțiunea **Customer Insight title:** și utilizați-o ca punct de pornire pentru titlul H1 pentru înțelegere.</span><span class="sxs-lookup"><span data-stu-id="ba27c-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="ba27c-113">Insights Alchemy trebuie să aibă doar un singur H1 în partea de sus sau se vor rupe în producție.</span><span class="sxs-lookup"><span data-stu-id="ba27c-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="ba27c-114">H2s nu redă niciuna dintre **bold** aceste convenții pentru a semnifica secțiuni separate.</span><span class="sxs-lookup"><span data-stu-id="ba27c-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="ba27c-115">Apoi, completați corpul de text utilizând schița de material din secțiunea Customer Insights a paginii de reguli Alchemy</span><span class="sxs-lookup"><span data-stu-id="ba27c-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="ba27c-116">Listele cu marcatori sunt în regulă</span><span class="sxs-lookup"><span data-stu-id="ba27c-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="ba27c-117">Și liste numerotate</span><span class="sxs-lookup"><span data-stu-id="ba27c-117">Numbered lists too</span></span>
    1. <span data-ttu-id="ba27c-118">**Aldin** și *cursiv* sunt a-OK</span><span class="sxs-lookup"><span data-stu-id="ba27c-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="ba27c-119">Linkurile trebuie să fie întotdeauna **"linkuri către web"/external** sau **Deep-linkuri către elemente de interfață utilizator**, nu către Linkuri interne.</span><span class="sxs-lookup"><span data-stu-id="ba27c-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="ba27c-120">Imaginile nu sunt acceptate oficial în acest moment, dar se află în foaia de parcurs.</span><span class="sxs-lookup"><span data-stu-id="ba27c-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="ba27c-121">Iar acest lucru este într-adevăr deja un pic prea lung.</span><span class="sxs-lookup"><span data-stu-id="ba27c-121">And this is really already a bit too long.</span></span> <span data-ttu-id="ba27c-122">Cea mai bună practică este de aproximativ 400 de caractere---------------------------------</span><span class="sxs-lookup"><span data-stu-id="ba27c-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="ba27c-123">După ce conținutul este gata, trageți-l la ramura în direct.</span><span class="sxs-lookup"><span data-stu-id="ba27c-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="ba27c-124">Apoi, accesați portalul pentru [parteneri Alchemy](https://alchemyportal.azurewebsites.net) și introduceți numele de fișier în câmpul URL.</span><span class="sxs-lookup"><span data-stu-id="ba27c-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 