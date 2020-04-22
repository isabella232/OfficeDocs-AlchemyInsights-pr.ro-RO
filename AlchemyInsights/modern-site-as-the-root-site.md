---
title: Site-ul modern ca site-ul rădăcină
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713803"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="a2d12-102">Site-ul modern ca site-ul rădăcină</span><span class="sxs-lookup"><span data-stu-id="a2d12-102">Modern site as root site</span></span>

<span data-ttu-id="a2d12-103">Am început să rollout o nouă caracteristică care vă va permite să [swap site-ul clasic rădăcină site-ul cu un site modern](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="a2d12-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="a2d12-104">Utilizați [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locația unui site cu un alt site în timp ce arhivați site-ul original.</span><span class="sxs-lookup"><span data-stu-id="a2d12-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="a2d12-105">Disponibil atât pentru site-ul de echipă (care nu este conectat la un grup), cât și pentru site-ul de comunicare.</span><span class="sxs-lookup"><span data-stu-id="a2d12-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="a2d12-106">Nu ștergeți site-ul rădăcină clasic pentru a crea un site de comunicare modern.</span><span class="sxs-lookup"><span data-stu-id="a2d12-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="a2d12-107">Acest lucru nu este acceptat de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a2d12-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="a2d12-108">Ștergerea site-ului rădăcină va face toate site-urile SharePoint din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="a2d12-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="a2d12-109">Vom comunica această caracteristică prin intermediul centrului de mesaje.</span><span class="sxs-lookup"><span data-stu-id="a2d12-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="a2d12-110">Ar trebui să vă așteptați ca caracteristica să fie activată în entitatea găzduită în scurt timp.</span><span class="sxs-lookup"><span data-stu-id="a2d12-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="a2d12-111">Probleme cunoscute cu site-uri de schimbare</span><span class="sxs-lookup"><span data-stu-id="a2d12-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="a2d12-112">Site-ul țintă poate returna o eroare "negăsit" (HTTP 404) pentru o perioadă scurtă de timp.</span><span class="sxs-lookup"><span data-stu-id="a2d12-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="a2d12-113">Conținutul va trebui recrawled pentru a actualiza indexul de căutare.</span><span class="sxs-lookup"><span data-stu-id="a2d12-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="a2d12-114">Nu există nici un pas manual necesar aici, acest lucru se va face în mod automat.</span><span class="sxs-lookup"><span data-stu-id="a2d12-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="a2d12-115">Orice lucru dependent de linkurile "statice" (cum ar fi sincronizarea fișierelor și fișierele OneNote) va trebui corectat manual.</span><span class="sxs-lookup"><span data-stu-id="a2d12-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="a2d12-116">Site-uri Project Server poate fi necesar să fie validate pentru a se asigura că acestea sunt încă asociate corect.</span><span class="sxs-lookup"><span data-stu-id="a2d12-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
