---
title: Salvarea site-ului sau a listei ca șablon
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727543"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="8b738-102">Salvarea site-ului sau a listei ca șablon</span><span class="sxs-lookup"><span data-stu-id="8b738-102">Save site or list as a template</span></span>

<span data-ttu-id="8b738-103">Șabloanele de site SharePoint sunt definiții predefinite proiectate în jurul unei anumite necesități de firmă.</span><span class="sxs-lookup"><span data-stu-id="8b738-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="8b738-104">Pentru mai multe informații, consultați [utilizarea șabloanelor pentru a crea diverse tipuri de site-uri SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="8b738-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="8b738-105">Iată câteva probleme comune/soluții cu privire la salvarea unui site sau a unei liste ca șablon în SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="8b738-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="8b738-106">**Butonul Salvare șablon de site/listă nu este disponibil sau lipsește**.</span><span class="sxs-lookup"><span data-stu-id="8b738-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="8b738-107">Administratorii vor trebui să permită un script particularizat pentru a activa caracteristicile șablonului.</span><span class="sxs-lookup"><span data-stu-id="8b738-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="8b738-108">Pentru pași detaliați, exemple și considerații, consultați [permiterea sau prevenirea scripturilor particularizate](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="8b738-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="8b738-109">Comanda Salvare site ca șablon nu este acceptată și poate provoca probleme pe site-uri care utilizează infrastructura de publicare SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="8b738-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="8b738-110">**Șablonul de site nu poate fi creat sau nu funcționează corect**</span><span class="sxs-lookup"><span data-stu-id="8b738-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="8b738-111">Șablonul poate fi lipsește o [caracteristică](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) și nu se va activa.</span><span class="sxs-lookup"><span data-stu-id="8b738-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="8b738-112">Dacă caracteristica nu este disponibilă pentru a fi activată în colecția de site-uri curentă, nu puteți utiliza șablonul de site pentru a crea un site.</span><span class="sxs-lookup"><span data-stu-id="8b738-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="8b738-113">Verificați dacă listele sau bibliotecile depășesc [pragul limită de vizualizare a listei](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de elemente 5000, deoarece acest lucru poate bloca crearea unui șablon de site.</span><span class="sxs-lookup"><span data-stu-id="8b738-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="8b738-114">Este posibil ca site-ul să utilizeze prea multe resurse și, prin urmare, șablonul de site depășește limita de 50 megaocteți (MO).</span><span class="sxs-lookup"><span data-stu-id="8b738-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="8b738-115">Există probleme la afișarea datelor dintr-o listă care utilizează o coloană de căutare.</span><span class="sxs-lookup"><span data-stu-id="8b738-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="8b738-116">Pentru mai multe informații, consultați [lista generate de șabloane nu afișează date din lista de căutare corectă din SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="8b738-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="8b738-117">Pentru mai multe informații detaliate despre problemele și soluțiile comune, consultați referințe, [Creați și utilizați șabloane de site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="8b738-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

