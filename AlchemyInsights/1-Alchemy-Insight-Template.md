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
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634516"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="7fed4-102">Necesare alchimie antet H1, H2 pe nu funcţionează.</span><span class="sxs-lookup"><span data-stu-id="7fed4-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="7fed4-103">Cele mai bune practici și liniile directoare pentru authoring de Alchemy:</span><span class="sxs-lookup"><span data-stu-id="7fed4-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="7fed4-104">**Cuib alchimie intuiţii în dosare**- acest lucru va rupe structura de URL-ul.</span><span class="sxs-lookup"><span data-stu-id="7fed4-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="7fed4-105">Suntem în căutarea în stabilirea acest lucru.</span><span class="sxs-lookup"><span data-stu-id="7fed4-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="7fed4-106">Fişierele din folderul **AlchemyInsights** trebuie să aibă regula ID-ul şi numele de regulă la [alchimie partener portal](https://alchemyportal.azurewebsites.net) în numele fişierului.</span><span class="sxs-lookup"><span data-stu-id="7fed4-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="7fed4-107">ex.</span><span class="sxs-lookup"><span data-stu-id="7fed4-107">ex.</span></span> <span data-ttu-id="7fed4-108">***976-How-to-Enable-Litigation-Hold***</span><span class="sxs-lookup"><span data-stu-id="7fed4-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="7fed4-109">Utiliza metadatele în partea de sus a acestui fișier ca șablon.</span><span class="sxs-lookup"><span data-stu-id="7fed4-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="7fed4-110">Nimic altceva nu este necesară.</span><span class="sxs-lookup"><span data-stu-id="7fed4-110">Nothing else is required.</span></span>
1. <span data-ttu-id="7fed4-111">În [alchimie partener portal](https://alchemyportal.azurewebsites.net), navigaţi în jos la secţiunea **titlu de carte de vizita clientului:** și care, ca începând cu un punct pentru H1 titlu pentru înţelegere.</span><span class="sxs-lookup"><span data-stu-id="7fed4-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="7fed4-112">Alchimia intuiţii trebuie să aibă doar un singur H1 la partea de sus sau se va intrerupe în producţie.</span><span class="sxs-lookup"><span data-stu-id="7fed4-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="7fed4-113">H2s nu face atât utilizarea **îndrăzneţ** sau alte convenții înseamnă secţiuni separate.</span><span class="sxs-lookup"><span data-stu-id="7fed4-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="7fed4-114">Apoi, completaţi în corpul textului folosind materiale de proiect în secţiunea clientului intuiţii a paginii de regulă de alchimie</span><span class="sxs-lookup"><span data-stu-id="7fed4-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="7fed4-115">Liste cu marcatori sunt bine</span><span class="sxs-lookup"><span data-stu-id="7fed4-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="7fed4-116">Liste numerotate prea</span><span class="sxs-lookup"><span data-stu-id="7fed4-116">Numbered lists too</span></span>
    1. <span data-ttu-id="7fed4-117">**Bold** şi *cursive* sunt un-OK</span><span class="sxs-lookup"><span data-stu-id="7fed4-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="7fed4-118">Link-uri ar trebui să fie întotdeauna **"link-uri la web" / extern** OR **adânc-link-uri la elemente de UI**, link-uri nu interne.</span><span class="sxs-lookup"><span data-stu-id="7fed4-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="7fed4-119">Şi acest lucru este într-adevăr deja un pic prea lung.</span><span class="sxs-lookup"><span data-stu-id="7fed4-119">And this is really already a bit too long.</span></span> <span data-ttu-id="7fed4-120">Cele mai bune practici este de aproximativ 400 de caractere---</span><span class="sxs-lookup"><span data-stu-id="7fed4-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="7fed4-121">Odată ce conţinutul este gata, trageţi-l la sucursala live.</span><span class="sxs-lookup"><span data-stu-id="7fed4-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="7fed4-122">Apoi, du-te la [portalului Partner de alchimie](https://alchemyportal.azurewebsites.net) şi introduceţi numele fişierului în câmpul URL-ul.</span><span class="sxs-lookup"><span data-stu-id="7fed4-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="7fed4-123">Asiguraţi-vă că Insight revizuite şi publicate spune "Da" şi apoi faceţi clic pe regulă de actualizare.</span><span class="sxs-lookup"><span data-stu-id="7fed4-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="7fed4-124">**(Acest lucru va arata mai frumoasa în noua versiune a portalului - eliberarea în curând.)** 
 ![url field](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="7fed4-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

