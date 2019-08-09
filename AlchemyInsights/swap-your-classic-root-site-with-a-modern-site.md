---
title: Swap vă clasic site-ul rădăcină, cu un site Modern
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270756"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="85ae6-102">Swap vă clasic site-ul rădăcină, cu un site Modern</span><span class="sxs-lookup"><span data-stu-id="85ae6-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="85ae6-103">În cazul în care mediul vostru a fost creat înainte de aprilie 2019, puteţi schimba site-ul rădăcină a unui site modern utilizând Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="85ae6-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="85ae6-104">Dacă aveţi un alt site pe care doriţi să o utilizaţi ca site-ul rădăcină, puteţi înlocui (swap) rădăcină site-ul cu ea.</span><span class="sxs-lookup"><span data-stu-id="85ae6-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="85ae6-105">Utilizaţi [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locaţia de un site cu un alt site în timp ce site-ul original de arhivare.</span><span class="sxs-lookup"><span data-stu-id="85ae6-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="85ae6-106">Disponibil pentru echipa site-ului (nu este conectat la un grup) şi de site-ul de comunicare.</span><span class="sxs-lookup"><span data-stu-id="85ae6-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="85ae6-107">Capabilităţi suplimentare vor fi introduse în curând care vă va permite să păstraţi folosind conţinut pe site-ul, dar conversia site-ul existent la un site de comunicare.</span><span class="sxs-lookup"><span data-stu-id="85ae6-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="85ae6-108">Aceste capabilităţi va fi lansat treptat.</span><span class="sxs-lookup"><span data-stu-id="85ae6-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="85ae6-109">Continuaţi pentru a verifica Office 365 centru de mesaje pentru actualizări.</span><span class="sxs-lookup"><span data-stu-id="85ae6-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="85ae6-110">Probleme cunoscute cu schimbarea site-uri</span><span class="sxs-lookup"><span data-stu-id="85ae6-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="85ae6-111">Site-ul ţintă poate returna o eroare "nu a fost găsit" (HTTP 404) pentru o perioadă scurtă de timp.</span><span class="sxs-lookup"><span data-stu-id="85ae6-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="85ae6-112">Conținutul va trebui să fie el scotocit din nou pentru a actualiza indexul de căutare.</span><span class="sxs-lookup"><span data-stu-id="85ae6-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="85ae6-113">Nu există nici un pas manuală necesară - acest lucru se va face automat.</span><span class="sxs-lookup"><span data-stu-id="85ae6-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="85ae6-114">Nimic depinde şi de link-uri "statice" (cum ar fi fişiere fişier sincronizare și OneNote) va trebui să manual corectate.</span><span class="sxs-lookup"><span data-stu-id="85ae6-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="85ae6-115">În cazul în care site-ul sursă a fost un site de ştiri organizaţionale, Actualizaţi URL-ul.</span><span class="sxs-lookup"><span data-stu-id="85ae6-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="85ae6-116">Obţineţi o listă de toate site-urile de ştiri organizatorice.</span><span class="sxs-lookup"><span data-stu-id="85ae6-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="85ae6-117">Proiect Server site-uri trebuie să fie validate pentru a se asigura că acestea sunt încă asociate corect.</span><span class="sxs-lookup"><span data-stu-id="85ae6-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





