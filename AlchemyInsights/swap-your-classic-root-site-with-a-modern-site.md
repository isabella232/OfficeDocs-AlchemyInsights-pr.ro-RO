---
title: Schimbați-vă site-ul rădăcină clasic cu un site modern
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741556"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="48958-102">Schimbați-vă site-ul rădăcină clasic cu un site modern</span><span class="sxs-lookup"><span data-stu-id="48958-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="48958-103">Dacă mediul a fost configurat înainte de aprilie 2019, puteți modifica site-ul rădăcină într-un site modern utilizând Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="48958-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="48958-104">Dacă aveți un alt site pe care doriți să îl utilizați ca site rădăcină, puteți înlocui [(schimba) site-ul rădăcină](https://docs.microsoft.com/sharepoint/modern-root-site) cu acesta.</span><span class="sxs-lookup"><span data-stu-id="48958-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="48958-105">Utilizați [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locația unui site cu un alt site în timp ce arhivați site-ul original.</span><span class="sxs-lookup"><span data-stu-id="48958-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="48958-106">Disponibil atât pentru site-ul de echipă (care nu este conectat la un grup), cât și pentru site-ul de comunicare.</span><span class="sxs-lookup"><span data-stu-id="48958-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="48958-107">Capacități suplimentare vor fi introduse în curând, care vă vor permite să continuați să utilizați conținutul de pe site, dar să convertiți site-ul existent într-un site de comunicare.</span><span class="sxs-lookup"><span data-stu-id="48958-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="48958-108">Aceste capabilități vor fi lansate treptat.</span><span class="sxs-lookup"><span data-stu-id="48958-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="48958-109">Continuați să verificați Centrul de mesaje pentru actualizări.</span><span class="sxs-lookup"><span data-stu-id="48958-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="48958-110">Probleme cunoscute cu site-uri de schimbare</span><span class="sxs-lookup"><span data-stu-id="48958-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="48958-111">Site-ul țintă poate returna o eroare "negăsit" (HTTP 404) pentru o perioadă scurtă de timp.</span><span class="sxs-lookup"><span data-stu-id="48958-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="48958-112">Conținutul va trebui recrawled pentru a actualiza indexul de căutare.</span><span class="sxs-lookup"><span data-stu-id="48958-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="48958-113">Nu există nici un pas manual necesar - acest lucru se va face în mod automat.</span><span class="sxs-lookup"><span data-stu-id="48958-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="48958-114">Orice lucru dependent de linkurile "statice" (cum ar fi sincronizarea fișierelor și fișierele OneNote) va trebui corectat manual.</span><span class="sxs-lookup"><span data-stu-id="48958-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="48958-115">Dacă site-ul sursă a fost un site de știri organizațional, actualizați URL-ul.</span><span class="sxs-lookup"><span data-stu-id="48958-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="48958-116">Obțineți o listă cu toate site-urile de știri organizaționale.</span><span class="sxs-lookup"><span data-stu-id="48958-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="48958-117">Site-uri Project Server poate fi necesar să fie validate pentru a se asigura că acestea sunt încă asociate corect.</span><span class="sxs-lookup"><span data-stu-id="48958-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
