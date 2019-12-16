---
title: Swap site-ul rădăcină clasic cu un site modern
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042939"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="bb698-102">Swap site-ul rădăcină clasic cu un site modern</span><span class="sxs-lookup"><span data-stu-id="bb698-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="bb698-103">Dacă mediul a fost configurat înainte de aprilie 2019, aveți posibilitatea să modificați site-ul rădăcină la un site modern utilizând Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="bb698-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="bb698-104">Dacă aveți un site diferit pe care doriți să-l utilizați ca site-ul rădăcină, puteți înlocui [(swap) site-ul rădăcină](https://docs.microsoft.com/sharepoint/modern-root-site) cu ea.</span><span class="sxs-lookup"><span data-stu-id="bb698-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="bb698-105">Utilizați [Invoke-,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locația unui site cu un alt site în timp ce arhivați site-ul original.</span><span class="sxs-lookup"><span data-stu-id="bb698-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="bb698-106">Disponibil pentru ambele site-uri de echipă (nu sunt conectate la un grup) și site-ul de comunicare.</span><span class="sxs-lookup"><span data-stu-id="bb698-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="bb698-107">Capacitățile suplimentare vor fi introduse în curând, care vă va permite să păstrați folosind conținutul de pe site-ul, dar converti site-ul existent la un site de comunicare.</span><span class="sxs-lookup"><span data-stu-id="bb698-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="bb698-108">Aceste capacități vor fi laminate treptat.</span><span class="sxs-lookup"><span data-stu-id="bb698-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="bb698-109">Continuați pentru a verifica Office 365 Message Center pentru actualizări.</span><span class="sxs-lookup"><span data-stu-id="bb698-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="bb698-110">Probleme cunoscute cu schimbarea site-uri</span><span class="sxs-lookup"><span data-stu-id="bb698-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="bb698-111">Site-ul țintă poate returna o eroare "nu a fost găsit" (HTTP 404) pentru o perioadă scurtă de timp.</span><span class="sxs-lookup"><span data-stu-id="bb698-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="bb698-112">Conținutul va trebui să fie scotocit din nou pentru a actualiza indexul de căutare.</span><span class="sxs-lookup"><span data-stu-id="bb698-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="bb698-113">Nu există nici un pas manual necesar-acest lucru se va face în mod automat.</span><span class="sxs-lookup"><span data-stu-id="bb698-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="bb698-114">Orice depinde de "static" link-uri (cum ar fi fișiere de sincronizare și fișiere OneNote) va trebui să fie corectate manual.</span><span class="sxs-lookup"><span data-stu-id="bb698-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="bb698-115">Dacă site-ul sursă a fost un site de știri organizaționale, actualizați URL-ul.</span><span class="sxs-lookup"><span data-stu-id="bb698-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="bb698-116">Obțineți o listă cu toate site-urile de știri organizatorice.</span><span class="sxs-lookup"><span data-stu-id="bb698-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="bb698-117">Site-uri de proiect Server poate fi necesar să fie validate pentru a se asigura că acestea sunt încă asociate corect.</span><span class="sxs-lookup"><span data-stu-id="bb698-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





