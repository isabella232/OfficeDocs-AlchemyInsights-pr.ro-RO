---
title: Crearea unui site în SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732248"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="ac4f4-102">Crearea de site-uri SharePoint utilizând șabloane</span><span class="sxs-lookup"><span data-stu-id="ac4f4-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="ac4f4-103">Capacitatea de a salva un site ca șablon nu este acceptată cu comunicațiile moderne sau cu site-urile de echipă.</span><span class="sxs-lookup"><span data-stu-id="ac4f4-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="ac4f4-104">Pentru mai multe informații despre utilizarea șabloanelor [, consultați Salvarea, descărcarea și încărcarea unui site SharePoint ca șablon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="ac4f4-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="ac4f4-105">Iată câteva probleme comune/soluții cu privire la salvarea unui site sau a unei liste ca șablon în SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="ac4f4-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="ac4f4-106">**Butonul Salvare șablon de site/listă nu este disponibil sau lipsește**</span><span class="sxs-lookup"><span data-stu-id="ac4f4-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="ac4f4-107">Administratorii vor trebui să permită un script particularizat pentru a activa caracteristicile șablonului.</span><span class="sxs-lookup"><span data-stu-id="ac4f4-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="ac4f4-108">Pentru pași detaliați, exemple și considerații, consultați</span><span class="sxs-lookup"><span data-stu-id="ac4f4-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="ac4f4-109">Permiterea sau prevenirea scripturilor particularizate</span><span class="sxs-lookup"><span data-stu-id="ac4f4-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="ac4f4-110">Comanda Salvare site ca șablon nu este acceptată și poate provoca probleme pe site-uri care utilizează infrastructura de publicare SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="ac4f4-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="ac4f4-111">**Șablonul de site nu poate fi creat sau nu funcționează corect**</span><span class="sxs-lookup"><span data-stu-id="ac4f4-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="ac4f4-112">Șablonul poate fi lipsește o [caracteristică](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) și nu se va activa.</span><span class="sxs-lookup"><span data-stu-id="ac4f4-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="ac4f4-113">Dacă caracteristica nu este disponibilă pentru a fi activată în colecția de site-uri curentă, nu puteți utiliza șablonul de site pentru a crea un site.</span><span class="sxs-lookup"><span data-stu-id="ac4f4-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="ac4f4-114">Verificați dacă listele sau bibliotecile depășesc [pragul limită de vizualizare a listei](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de elemente 5000, deoarece acest lucru poate bloca crearea unui șablon de site.</span><span class="sxs-lookup"><span data-stu-id="ac4f4-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="ac4f4-115">Este posibil ca site-ul să utilizeze prea multe resurse și, prin urmare, șablonul de site depășește limita de 50 MB.</span><span class="sxs-lookup"><span data-stu-id="ac4f4-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="ac4f4-116">Există probleme la afișarea datelor dintr-o listă care utilizează o coloană de căutare.</span><span class="sxs-lookup"><span data-stu-id="ac4f4-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="ac4f4-117">Pentru mai multe informații, consultați [lista generate de șabloane nu afișează date din lista de căutare corectă din SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="ac4f4-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="ac4f4-118">Pentru mai multe informații detaliate despre problemele și soluțiile comune, consultați [crearea și utilizarea șabloanelor de site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="ac4f4-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



