---
title: Site modern ca site rădăcină
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666882"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="24064-102">Site modern ca site rădăcină</span><span class="sxs-lookup"><span data-stu-id="24064-102">Modern site as root site</span></span>

<span data-ttu-id="24064-103">Am început să lansăm o nouă caracteristică care vă va permite să vă swap site-ul de [rădăcină clasic site cu un site modern](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="24064-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="24064-104">Utilizați [invocare-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locația unui site cu alt site în timp ce arhivați site-ul original.</span><span class="sxs-lookup"><span data-stu-id="24064-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="24064-105">Disponibil pentru ambele site-uri de echipă (neconectat la un grup) și site de comunicare.</span><span class="sxs-lookup"><span data-stu-id="24064-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="24064-106">Nu ștergeți site-ul rădăcină clasic pentru a crea un site de comunicare modern.</span><span class="sxs-lookup"><span data-stu-id="24064-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="24064-107">Acest lucru nu este acceptat de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="24064-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="24064-108">Ștergerea site-ului rădăcină va face toate site-urile SharePoint din organizație inaccesibile pentru toți utilizatorii, până când restaurați site-ul sau creați un site nou la același URL.</span><span class="sxs-lookup"><span data-stu-id="24064-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="24064-109">Vom comunica această caracteristică prin centrul de mesaje.</span><span class="sxs-lookup"><span data-stu-id="24064-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="24064-110">Trebuie să vă așteptați ca caracteristica să fie activată în entitatea găzduită în scurt timp.</span><span class="sxs-lookup"><span data-stu-id="24064-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="24064-111">Probleme cunoscute cu înlocuirea site-urilor</span><span class="sxs-lookup"><span data-stu-id="24064-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="24064-112">Site-ul țintă poate returna o eroare "nu s-a găsit" (HTTP 404) pentru o perioadă scurtă de timp.</span><span class="sxs-lookup"><span data-stu-id="24064-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="24064-113">Conținutul va trebui să fie rescotocit pentru a actualiza indexul de căutare.</span><span class="sxs-lookup"><span data-stu-id="24064-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="24064-114">Nu este necesar un pas manual aici, acesta va fi efectuat automat.</span><span class="sxs-lookup"><span data-stu-id="24064-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="24064-115">Orice dependență de linkuri "statice" (cum ar fi sincronizarea fișierelor și fișierele OneNote) va trebui să fie corectată manual.</span><span class="sxs-lookup"><span data-stu-id="24064-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="24064-116">Site-urile Project Server pot necesita validarea pentru a vă asigura că acestea sunt încă asociate corect.</span><span class="sxs-lookup"><span data-stu-id="24064-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
