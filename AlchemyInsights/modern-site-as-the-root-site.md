---
title: Site-ul modernă ca site-ul rădăcină
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232727"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="65aa7-102">Site-ul modernă ca site-ul rădăcină</span><span class="sxs-lookup"><span data-stu-id="65aa7-102">Modern site as root site</span></span>

<span data-ttu-id="65aa7-103">Am început să rollout o caracteristică nouă care vă va permite să vă site-ul clasic site-ul rădăcină, cu un site modern de swap.</span><span class="sxs-lookup"><span data-stu-id="65aa7-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="65aa7-104">Utilizaţi [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locaţia de un site cu un alt site în timp ce site-ul original de arhivare.</span><span class="sxs-lookup"><span data-stu-id="65aa7-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="65aa7-105">Disponibil pentru echipa site-ului (nu este conectat la un grup) şi de site-ul de comunicare.</span><span class="sxs-lookup"><span data-stu-id="65aa7-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="65aa7-106">Imposibil de șters site-ul clasic rădăcină pentru a crea un Site de comunicare moderne.</span><span class="sxs-lookup"><span data-stu-id="65aa7-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="65aa7-107">Acest lucru nu este acceptată de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="65aa7-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="65aa7-108">Ştergerea site-ul rădăcină va face toate site-urile SharePoint din organizaţie inaccesibile pentru toţi utilizatorii, până la restaurarea site-ul sau de a crea un site nou la aceeaşi adresă URL.</span><span class="sxs-lookup"><span data-stu-id="65aa7-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="65aa7-109">Ne veţi fi comunicarea această caracteristică prin centrul de mesaje.</span><span class="sxs-lookup"><span data-stu-id="65aa7-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="65aa7-110">Ar trebui să aşteptaţi caracteristică să fie pornit în chiriaşul dumneavoastră la scurt timp.</span><span class="sxs-lookup"><span data-stu-id="65aa7-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="65aa7-111">Probleme cunoscute cu schimbarea site-uri</span><span class="sxs-lookup"><span data-stu-id="65aa7-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="65aa7-112">Site-ul ţintă poate returna o eroare "nu a fost găsit" (HTTP 404) pentru o perioadă scurtă de timp.</span><span class="sxs-lookup"><span data-stu-id="65aa7-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="65aa7-113">Conținutul va trebui să fie el scotocit din nou pentru a actualiza indexul de căutare.</span><span class="sxs-lookup"><span data-stu-id="65aa7-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="65aa7-114">Nu există nici un manual pas necesar aici, acest lucru se va face automat.</span><span class="sxs-lookup"><span data-stu-id="65aa7-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="65aa7-115">Nimic depinde şi de link-uri "statice" (cum ar fi fişiere fişier sincronizare și OneNote) va trebui să manual corectate.</span><span class="sxs-lookup"><span data-stu-id="65aa7-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="65aa7-116">Proiect Server site-uri trebuie să fie validate pentru a se asigura că acestea sunt încă asociate corect.</span><span class="sxs-lookup"><span data-stu-id="65aa7-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
