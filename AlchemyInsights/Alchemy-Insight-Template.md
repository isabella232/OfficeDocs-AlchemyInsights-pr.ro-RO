---
title: la fel ca numele de fișier este cel mai bun
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750982"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="b9bab-102">"Obligatoriu Alchemy Header H1, H2 nu funcționează."</span><span class="sxs-lookup"><span data-stu-id="b9bab-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="b9bab-103">Cele mai bune practici și orientări pentru alchimie autor:</span><span class="sxs-lookup"><span data-stu-id="b9bab-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="b9bab-104">**Nu cuib Alchemy Insights în foldere**- acest lucru va rupe structura URL-ul.</span><span class="sxs-lookup"><span data-stu-id="b9bab-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="b9bab-105">Căutăm să reparăm asta.</span><span class="sxs-lookup"><span data-stu-id="b9bab-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="b9bab-106">Fișierele din folderul **AlchemyInsights** ar trebui să aibă nume de fișiere minuscule cu cratime pentru spațiiex.</span><span class="sxs-lookup"><span data-stu-id="b9bab-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="b9bab-107">***cum să-enable-litigation-hold***.</span><span class="sxs-lookup"><span data-stu-id="b9bab-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="b9bab-108">Includeți ID-ul de regulă sau ID-ul de găleată din [portalul Alchemy Partner](https://alchemyportal.azurewebsites.net) în câmpul ms.custom.</span><span class="sxs-lookup"><span data-stu-id="b9bab-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="b9bab-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="b9bab-109">ex.</span></span> <span data-ttu-id="b9bab-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="b9bab-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="b9bab-111">Utilizați restul metadatelor din partea de sus a acestui fișier ca șablon.</span><span class="sxs-lookup"><span data-stu-id="b9bab-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="b9bab-112">În [portalul Alchemy Partner](https://alchemyportal.azurewebsites.net), navigați în jos la secțiunea **Customer Insight Title:** și utilizați-o ca punct de plecare pentru titlul H1 pentru înțelegere.</span><span class="sxs-lookup"><span data-stu-id="b9bab-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="b9bab-113">Alchemy Insights trebuie să aibă doar un singur H1 în partea de sus sau se va rupe în producție.</span><span class="sxs-lookup"><span data-stu-id="b9bab-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="b9bab-114">H2-urile nu redau nici așa că utilizați convenții **aldine** sau alte convenții pentru a semnifica secțiuni separate.</span><span class="sxs-lookup"><span data-stu-id="b9bab-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="b9bab-115">Apoi, completați textul corpului utilizând materialul schiță din secțiunea Customer Insights a paginii Alchemy Rule</span><span class="sxs-lookup"><span data-stu-id="b9bab-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="b9bab-116">Listele cu marcatori sunt în regulă</span><span class="sxs-lookup"><span data-stu-id="b9bab-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="b9bab-117">Liste numerotate prea</span><span class="sxs-lookup"><span data-stu-id="b9bab-117">Numbered lists too</span></span>
    1. <span data-ttu-id="b9bab-118">**Bold** și *cursiv* sunt a-ok</span><span class="sxs-lookup"><span data-stu-id="b9bab-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="b9bab-119">Link-uri ar trebui să fie întotdeauna fie **"link-uri către web"/extern** sau **deep-link-uri către elemente ui, nu link-uri**interne.</span><span class="sxs-lookup"><span data-stu-id="b9bab-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="b9bab-120">Imaginile nu sunt acceptate oficial în acest moment, dar este pe foaia de parcurs.</span><span class="sxs-lookup"><span data-stu-id="b9bab-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="b9bab-121">Și asta e deja un pic prea lung.</span><span class="sxs-lookup"><span data-stu-id="b9bab-121">And this is really already a bit too long.</span></span> <span data-ttu-id="b9bab-122">Cele mai bune practici este de aproximativ 400 de caractere ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="b9bab-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="b9bab-123">Odată ce conținutul este gata, trageți-l la ramura live.</span><span class="sxs-lookup"><span data-stu-id="b9bab-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="b9bab-124">Apoi, accesați [portalul Alchemy Partner](https://alchemyportal.azurewebsites.net) și introduceți numele fișierului în câmpul URL.</span><span class="sxs-lookup"><span data-stu-id="b9bab-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 