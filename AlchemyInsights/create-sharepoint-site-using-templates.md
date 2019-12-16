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
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052481"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="98a89-102">Crearea de site-uri SharePoint utilizând șabloane</span><span class="sxs-lookup"><span data-stu-id="98a89-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="98a89-103">Șabloanele de site SharePoint sunt definiții predefinite proiectate în jurul unei nevoi speciale de afaceri.</span><span class="sxs-lookup"><span data-stu-id="98a89-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="98a89-104">Pentru mai multe informații, consultați [utilizarea șabloanelor pentru a crea diferite tipuri de site-uri SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="98a89-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="98a89-105">Iată câteva probleme/soluții obișnuite privind salvarea unui site sau a unei liste ca șablon în SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="98a89-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="98a89-106">**Salvați butonul șablon de site/listă nu este disponibil sau lipsește**</span><span class="sxs-lookup"><span data-stu-id="98a89-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="98a89-107">Administratorii vor trebui să permită script particularizat pentru a activa caracteristicile șablonului.</span><span class="sxs-lookup"><span data-stu-id="98a89-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="98a89-108">Pentru pași detaliați, exemplele și considerațiile</span><span class="sxs-lookup"><span data-stu-id="98a89-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="98a89-109">Permiteți sau împiedicați scriptul particularizat</span><span class="sxs-lookup"><span data-stu-id="98a89-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="98a89-110">Comanda Salvare site ca șablon nu este acceptată și poate provoca probleme pe site-uri care utilizează infrastructura de publicare SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="98a89-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="98a89-111">**Imposibil de creat șablonul de site sau nu funcționează corect**</span><span class="sxs-lookup"><span data-stu-id="98a89-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="98a89-112">Este posibil ca șablonul să lipsească o [caracteristică](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) și să nu se activeze.</span><span class="sxs-lookup"><span data-stu-id="98a89-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="98a89-113">Dacă caracteristica nu este disponibilă pentru a activa în colecția de site-uri curentă, nu se poate utiliza șablonul de site-ul pentru a crea un site.</span><span class="sxs-lookup"><span data-stu-id="98a89-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="98a89-114">Verificați pentru a vedea dacă orice liste sau biblioteci depășesc [pragul de vedere listă limită](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 elemente, deoarece acest lucru poate bloca crearea unui șablon de site-ul.</span><span class="sxs-lookup"><span data-stu-id="98a89-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="98a89-115">Site-ul poate fi folosind prea multe resurse și, prin urmare, șablonul de site-ul depășește limita de 50 MB.</span><span class="sxs-lookup"><span data-stu-id="98a89-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="98a89-116">Există probleme la afișarea datelor dintr-o listă care utilizează o coloană de căutare.</span><span class="sxs-lookup"><span data-stu-id="98a89-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="98a89-117">Pentru mai multe informații, consultați [șablon generat listă nu afișează date din Listă tabel de căutare corectă în SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="98a89-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="98a89-118">Pentru informații mai detaliate despre problemele și soluțiile obișnuite, consultați [crearea și utilizarea șabloanelor de site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="98a89-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



