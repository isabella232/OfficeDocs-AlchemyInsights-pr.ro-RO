---
title: Site-ul modern ca site-ul rădăcină
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753916"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="91ec3-102">Site-ul modern ca rădăcină site-ului</span><span class="sxs-lookup"><span data-stu-id="91ec3-102">Modern site as root site</span></span>

<span data-ttu-id="91ec3-103">Am început să rollout o nouă facilitate care vă va permite să swap site-ul site-ul [clasic rădăcină cu un site modern](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="91ec3-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="91ec3-104">Utilizați [Invoke-,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locația unui site cu un alt site în timp ce arhivați site-ul original.</span><span class="sxs-lookup"><span data-stu-id="91ec3-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="91ec3-105">Disponibil pentru ambele site-uri de echipă (nu sunt conectate la un grup) și site-ul de comunicare.</span><span class="sxs-lookup"><span data-stu-id="91ec3-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="91ec3-106">Nu ștergeți site-ul rădăcină clasic pentru a crea un site modern de comunicare.</span><span class="sxs-lookup"><span data-stu-id="91ec3-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="91ec3-107">Acest lucru nu este acceptat de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="91ec3-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="91ec3-108">Ștergerea site-ului rădăcină va face toate site-urile SharePoint din organizație inaccesibile tuturor utilizatorilor, până când restaurați site-ul sau creați un site nou la același URL.</span><span class="sxs-lookup"><span data-stu-id="91ec3-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="91ec3-109">Vom comunica această caracteristică prin intermediul centrului de mesaje.</span><span class="sxs-lookup"><span data-stu-id="91ec3-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="91ec3-110">Trebuie să vă așteptați ca funcția să fie activată în curând în chiriaș.</span><span class="sxs-lookup"><span data-stu-id="91ec3-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="91ec3-111">Probleme cunoscute cu schimbarea site-uri</span><span class="sxs-lookup"><span data-stu-id="91ec3-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="91ec3-112">Site-ul țintă poate returna o eroare "nu a fost găsit" (HTTP 404) pentru o perioadă scurtă de timp.</span><span class="sxs-lookup"><span data-stu-id="91ec3-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="91ec3-113">Conținutul va trebui să fie scotocit din nou pentru a actualiza indexul de căutare.</span><span class="sxs-lookup"><span data-stu-id="91ec3-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="91ec3-114">Nu există nici un pas manual necesar aici, acest lucru se va face în mod automat.</span><span class="sxs-lookup"><span data-stu-id="91ec3-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="91ec3-115">Orice depinde de "static" link-uri (cum ar fi fișiere de sincronizare și fișiere OneNote) va trebui să fie corectate manual.</span><span class="sxs-lookup"><span data-stu-id="91ec3-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="91ec3-116">Site-uri de proiect Server poate fi necesar să fie validate pentru a se asigura că acestea sunt încă asociate corect.</span><span class="sxs-lookup"><span data-stu-id="91ec3-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
