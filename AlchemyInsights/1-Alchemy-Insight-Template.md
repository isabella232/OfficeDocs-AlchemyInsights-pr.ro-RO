---
title: 'acelasi ca numele fişierului este cel mai bun [regula #-Descriere]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 01d8b03209e734f1218de61d964524b1b9e1d044
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939315"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="2a04a-102">Necesare alchimie antet H1, H2 pe nu funcţionează.</span><span class="sxs-lookup"><span data-stu-id="2a04a-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="2a04a-103">Cele mai bune practici și liniile directoare pentru authoring de Alchemy:</span><span class="sxs-lookup"><span data-stu-id="2a04a-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="2a04a-p101">**Cuib alchimie intuiţii în dosare**- acest lucru va rupe structura de URL-ul. Suntem în căutarea în stabilirea acest lucru.</span><span class="sxs-lookup"><span data-stu-id="2a04a-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="2a04a-106">Fişierele din folderul **AlchemyInsights** trebuie să aibă regula ID-ul şi numele de regulă la [alchimie partener portal](https://alchemyportal.azurewebsites.net) în numele fişierului.</span><span class="sxs-lookup"><span data-stu-id="2a04a-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="2a04a-p102">ex. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="2a04a-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="2a04a-p103">Utiliza metadatele în partea de sus a acestui fișier ca șablon. Nimic altceva nu este necesară.</span><span class="sxs-lookup"><span data-stu-id="2a04a-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="2a04a-111">În [alchimie partener portal](https://alchemyportal.azurewebsites.net), navigaţi în jos la secţiunea **titlu de carte de vizita clientului:** și care, ca începând cu un punct pentru H1 titlu pentru înţelegere.</span><span class="sxs-lookup"><span data-stu-id="2a04a-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="2a04a-p104">Alchimia intuiţii trebuie să aibă doar un singur H1 la partea de sus sau se va intrerupe în producţie. H2s nu face atât utilizarea **îndrăzneţ** sau alte convenții înseamnă secţiuni separate.</span><span class="sxs-lookup"><span data-stu-id="2a04a-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="2a04a-114">Apoi, completaţi în corpul textului folosind materiale de proiect în secţiunea clientului intuiţii a paginii de regulă de alchimie</span><span class="sxs-lookup"><span data-stu-id="2a04a-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="2a04a-115">Liste cu marcatori sunt bine</span><span class="sxs-lookup"><span data-stu-id="2a04a-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="2a04a-116">Liste numerotate prea</span><span class="sxs-lookup"><span data-stu-id="2a04a-116">Numbered lists too</span></span>
    1. <span data-ttu-id="2a04a-117">**Bold** şi *cursive* sunt un-OK</span><span class="sxs-lookup"><span data-stu-id="2a04a-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="2a04a-118">Link-uri ar trebui să fie întotdeauna **"link-uri la web" / extern** OR **adânc-link-uri la elemente de UI**, link-uri nu interne.</span><span class="sxs-lookup"><span data-stu-id="2a04a-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="2a04a-p105">Şi acest lucru este într-adevăr deja un pic prea lung. Cele mai bune practici este de aproximativ 400 de caractere---</span><span class="sxs-lookup"><span data-stu-id="2a04a-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="2a04a-p106">Odată ce conţinutul este gata, trageţi-l la sucursala live. Apoi, du-te la [portalului Partner de alchimie](https://alchemyportal.azurewebsites.net) şi introduceţi numele fişierului în câmpul URL-ul. Asiguraţi-vă că Insight revizuite şi publicate spune "Da" şi apoi faceţi clic pe regulă de actualizare. **(Acest lucru va arata mai frumoasa în noua versiune a portalului - eliberarea în curând.)** 
 ![url field](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="2a04a-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

