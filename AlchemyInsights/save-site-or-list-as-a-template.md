---
title: Salvare listă sau site-ul ca un şablon
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 73a32536995a604c734393c2300b4c9bb507e2b2
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770539"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="bf7e6-102">Salvare listă sau site-ul ca un şablon</span><span class="sxs-lookup"><span data-stu-id="bf7e6-102">Save site or list as a template</span></span>

<span data-ttu-id="bf7e6-103">Șabloanele de site SharePoint sunt precompilate definiţii concepute în jurul o afacere special nevoie.</span><span class="sxs-lookup"><span data-stu-id="bf7e6-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="bf7e6-104">Pentru informaţii suplimentare, consultaţi [utilizarea template-uri pentru a crea diferite tipuri de site-uri SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="bf7e6-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="bf7e6-105">Aici sunt unele probleme/solutii comune cu privire la salvarea un site-ul sau lista ca şablon în SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="bf7e6-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="bf7e6-106">**Salvaţi site/listă şablon buton este nu folositor sau lipsă**.</span><span class="sxs-lookup"><span data-stu-id="bf7e6-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="bf7e6-107">Administratorii va trebui să permite script-ul personalizat pentru a activa caracteristicile şablon.</span><span class="sxs-lookup"><span data-stu-id="bf7e6-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="bf7e6-108">Pentru măsurile detaliate, exemple şi consideraţii [permite sau împiedică script-ul personalizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="bf7e6-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="bf7e6-109">Site-ul salvaţi ca şablon de comandă nu este acceptată şi pot provoca probleme de pe site-urile care folosesc infrastructura de publicare SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="bf7e6-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="bf7e6-110">**Șablonul de site-ul nu poate fi creat sau nu funcţionează corect**</span><span class="sxs-lookup"><span data-stu-id="bf7e6-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="bf7e6-111">Poate să lipsească o [caracteristica](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) si nu se va activa.</span><span class="sxs-lookup"><span data-stu-id="bf7e6-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="bf7e6-112">Dacă funcţia nu este disponibilă pentru a activa în colecția de site-ul curent, se poate utiliza site-ul şablon pentru a crea un site.</span><span class="sxs-lookup"><span data-stu-id="bf7e6-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="bf7e6-113">Verificaţi pentru a vedea dacă orice liste sau biblioteci depăşi [Prag limită de vizualizare listă](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 de articole ca acest lucru poate bloca crearea unui şablon de site-ul.</span><span class="sxs-lookup"><span data-stu-id="bf7e6-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="bf7e6-114">Site-ul poate folosi prea multe resurse si, prin urmare, site-ul şablon depășește limita de 50 megabyte (MB).</span><span class="sxs-lookup"><span data-stu-id="bf7e6-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="bf7e6-115">Există probleme afişarea datelor dintr-o listă care utilizează o coloană de căutare.</span><span class="sxs-lookup"><span data-stu-id="bf7e6-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="bf7e6-116">Pentru informaţii suplimentare, consultaţi [generat şablon listă nu afişează datele din lista de căutare corectă în SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="bf7e6-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="bf7e6-117">Pentru informaţii mai detaliate pe probleme comune şi soluţii, vă rugăm să referinţă, [crearea şi utilizarea site-ul template-uri](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="bf7e6-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

