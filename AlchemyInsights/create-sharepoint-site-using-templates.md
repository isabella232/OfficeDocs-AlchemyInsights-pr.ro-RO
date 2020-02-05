---
title: Crearea unui site în SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770435"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="708c3-102">Crearea site-urilor SharePoint utilizând șabloane</span><span class="sxs-lookup"><span data-stu-id="708c3-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="708c3-103">Capacitatea de a salva un site ca șablon nu este acceptată cu site-uri moderne de comunicare sau de echipă.</span><span class="sxs-lookup"><span data-stu-id="708c3-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="708c3-104">Pentru mai multe informații despre utilizarea șabloanelor, consultați [Salvarea, descărcarea și încărcarea unui site SharePoint ca șablon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="708c3-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="708c3-105">Iată câteva probleme/soluții obișnuite în ceea ce privește salvarea unui site sau a unei liste ca șablon în Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="708c3-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="708c3-106">**Butonul Salvare șablon site/listă nu este disponibil sau lipsește**</span><span class="sxs-lookup"><span data-stu-id="708c3-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="708c3-107">Administratorii vor trebui să permită script personalizat pentru a activa caracteristicile șablonului.</span><span class="sxs-lookup"><span data-stu-id="708c3-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="708c3-108">Pentru pași detaliați, exemple și considerații, a se vedea</span><span class="sxs-lookup"><span data-stu-id="708c3-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="708c3-109">Permiterea sau prevenirea scriptului particularizat</span><span class="sxs-lookup"><span data-stu-id="708c3-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="708c3-110">Comanda Salvare site-ul ca șablon nu este acceptată și poate provoca probleme pe site-uri care utilizează infrastructura de publicare SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="708c3-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="708c3-111">**Șablonul de site nu se poate crea sau nu funcționează corect**</span><span class="sxs-lookup"><span data-stu-id="708c3-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="708c3-112">Este posibil ca șablonul să lipsească o [caracteristică](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) și să nu se activeze.</span><span class="sxs-lookup"><span data-stu-id="708c3-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="708c3-113">Dacă caracteristica nu este disponibilă pentru activare în colecția de site-uri curentă, aveți posibilitatea să utilizați șablonul de site pentru a crea un site.</span><span class="sxs-lookup"><span data-stu-id="708c3-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="708c3-114">Verificați dacă listele sau bibliotecile depășesc [pragul limită](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de vizualizare listă de 5000 de elemente, deoarece acest lucru poate bloca crearea unui șablon de site.</span><span class="sxs-lookup"><span data-stu-id="708c3-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="708c3-115">Site-ul poate fi folosind prea multe resurse și, prin urmare, șablonul de site-ul depășește limita de 50 MB.</span><span class="sxs-lookup"><span data-stu-id="708c3-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="708c3-116">Există probleme la afișarea datelor dintr-o listă care utilizează o coloană de căutare.</span><span class="sxs-lookup"><span data-stu-id="708c3-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="708c3-117">Pentru mai multe informații, consultați [Lista generată de șabloane nu afișează date din lista](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)de căutare corectă din SharePoint Online .</span><span class="sxs-lookup"><span data-stu-id="708c3-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="708c3-118">Pentru informații mai detaliate despre problemele și soluțiile obișnuite, verificați [Creați și utilizați șabloane de site.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)</span><span class="sxs-lookup"><span data-stu-id="708c3-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



