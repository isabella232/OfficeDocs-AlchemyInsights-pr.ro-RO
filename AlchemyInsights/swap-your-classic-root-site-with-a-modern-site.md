---
title: Swap site-ul rădăcină clasic cu un site modern
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691191"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="f2ff9-102">Swap site-ul rădăcină clasic cu un site modern</span><span class="sxs-lookup"><span data-stu-id="f2ff9-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="f2ff9-103">Dacă mediul a fost configurat înainte de aprilie 2019, puteți să modificați site-ul rădăcină la un site modern, utilizând Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="f2ff9-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="f2ff9-104">Dacă aveți un alt site pe care doriți să-l utilizați ca site rădăcină, puteți înlocui [(swap) site-ul rădăcină](https://docs.microsoft.com/sharepoint/modern-root-site) cu acesta.</span><span class="sxs-lookup"><span data-stu-id="f2ff9-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="f2ff9-105">Utilizați [invocare-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locația unui site cu alt site în timp ce arhivați site-ul original.</span><span class="sxs-lookup"><span data-stu-id="f2ff9-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="f2ff9-106">Disponibil pentru ambele site-uri de echipă (neconectat la un grup) și site de comunicare.</span><span class="sxs-lookup"><span data-stu-id="f2ff9-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="f2ff9-107">În curând vor fi introduse capacități suplimentare care vă vor permite să continuați să utilizați conținutul de pe site, dar să efectuați conversia site-ului existent pe un site de comunicare.</span><span class="sxs-lookup"><span data-stu-id="f2ff9-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="f2ff9-108">Aceste capacități vor fi derulate treptat.</span><span class="sxs-lookup"><span data-stu-id="f2ff9-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="f2ff9-109">Continuați să verificați Centrul de mesaje pentru actualizări.</span><span class="sxs-lookup"><span data-stu-id="f2ff9-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="f2ff9-110">Probleme cunoscute cu înlocuirea site-urilor</span><span class="sxs-lookup"><span data-stu-id="f2ff9-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="f2ff9-111">Site-ul țintă poate returna o eroare "nu s-a găsit" (HTTP 404) pentru o perioadă scurtă de timp.</span><span class="sxs-lookup"><span data-stu-id="f2ff9-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="f2ff9-112">Conținutul va trebui să fie rescotocit pentru a actualiza indexul de căutare.</span><span class="sxs-lookup"><span data-stu-id="f2ff9-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="f2ff9-113">Nu este necesar un pas manual-acest lucru se va face automat.</span><span class="sxs-lookup"><span data-stu-id="f2ff9-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="f2ff9-114">Orice dependență de linkuri "statice" (cum ar fi sincronizarea fișierelor și fișierele OneNote) va trebui să fie corectată manual.</span><span class="sxs-lookup"><span data-stu-id="f2ff9-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="f2ff9-115">Dacă site-ul sursă a fost un site de știri organizațional, actualizați URL-ul.</span><span class="sxs-lookup"><span data-stu-id="f2ff9-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="f2ff9-116">Obțineți o listă cu toate site-urile de știri organizaționale.</span><span class="sxs-lookup"><span data-stu-id="f2ff9-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="f2ff9-117">Site-urile Project Server pot necesita validarea pentru a vă asigura că acestea sunt încă asociate corect.</span><span class="sxs-lookup"><span data-stu-id="f2ff9-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
