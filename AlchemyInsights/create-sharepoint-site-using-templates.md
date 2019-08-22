---
title: Creaţi un site SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 7c24a0cf3bcae0f2780c1cb33c911cb38c1ca5cb
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515010"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="fd1db-102">Creare site-uri SharePoint folosind template-uri</span><span class="sxs-lookup"><span data-stu-id="fd1db-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="fd1db-103">Șabloanele de site SharePoint sunt precompilate definiţii concepute în jurul o afacere special nevoie.</span><span class="sxs-lookup"><span data-stu-id="fd1db-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="fd1db-104">Pentru informaţii suplimentare, consultaţi [utilizarea template-uri pentru a crea diferite tipuri de site-uri SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="fd1db-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="fd1db-105">Aici sunt unele probleme/solutii comune cu privire la salvarea un site-ul sau lista ca şablon în Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="fd1db-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="fd1db-106">**Salva/lista de site-ul şablon buton nu este disponibil sau lipsă**</span><span class="sxs-lookup"><span data-stu-id="fd1db-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="fd1db-107">Administratorii va trebui să permite script-ul personalizat pentru a activa caracteristicile şablon.</span><span class="sxs-lookup"><span data-stu-id="fd1db-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="fd1db-108">Pentru măsurile detaliate, consultaţi exemple şi consideraţii</span><span class="sxs-lookup"><span data-stu-id="fd1db-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="fd1db-109">Permite sau nu script-ul personalizat</span><span class="sxs-lookup"><span data-stu-id="fd1db-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="fd1db-110">Site-ul salvaţi ca şablon de comandă nu este acceptată şi pot provoca probleme de pe site-urile care folosesc infrastructura de publicare SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="fd1db-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="fd1db-111">**Șablonul de site-ul nu poate fi creat sau nu funcţionează corect**</span><span class="sxs-lookup"><span data-stu-id="fd1db-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="fd1db-112">Poate să lipsească o [caracteristica](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) si nu se va activa.</span><span class="sxs-lookup"><span data-stu-id="fd1db-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="fd1db-113">Dacă funcţia nu este disponibilă pentru a activa în colecția de site-ul curent, se poate utiliza site-ul şablon pentru a crea un site.</span><span class="sxs-lookup"><span data-stu-id="fd1db-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="fd1db-114">Verificaţi pentru a vedea dacă orice liste sau biblioteci depăşi [Prag limită de vizualizare listă](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 de articole ca acest lucru poate bloca crearea unui şablon de site-ul.</span><span class="sxs-lookup"><span data-stu-id="fd1db-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="fd1db-115">Site-ul poate folosi prea multe resurse si, prin urmare, site-ul şablon depășește limita de 50 MB.</span><span class="sxs-lookup"><span data-stu-id="fd1db-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="fd1db-116">Există probleme afişarea datelor dintr-o listă care utilizează o coloană de căutare.</span><span class="sxs-lookup"><span data-stu-id="fd1db-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="fd1db-117">Pentru informaţii suplimentare, consultaţi [generat şablon listă nu afişează datele din lista de căutare corectă în SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="fd1db-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="fd1db-118">Pentru informaţii mai detaliate pe probleme comune şi soluţii, vă rugăm să verificaţi [crearea şi utilizarea site-ul template-uri](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="fd1db-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



