---
title: Limitare SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931238"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="57276-102">Limitare SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="57276-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="57276-103">**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal.</span><span class="sxs-lookup"><span data-stu-id="57276-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="57276-104">Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă.</span><span class="sxs-lookup"><span data-stu-id="57276-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="57276-105">În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.</span><span class="sxs-lookup"><span data-stu-id="57276-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="57276-106">În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii.</span><span class="sxs-lookup"><span data-stu-id="57276-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="57276-107">Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade.</span><span class="sxs-lookup"><span data-stu-id="57276-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="57276-108">Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.</span><span class="sxs-lookup"><span data-stu-id="57276-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="57276-109">**503 server este ocupat de eroare**</span><span class="sxs-lookup"><span data-stu-id="57276-109">**503 server is busy error**</span></span>

<span data-ttu-id="57276-110">Utilizatorii pot primi un server 503 este ocupat eroare atunci când încercați să navigați la site-uri SharePoint sau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="57276-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="57276-111">Această eroare poate fi cauzată de limitare în cadrul serviciului SharePoint.</span><span class="sxs-lookup"><span data-stu-id="57276-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="57276-112">SharePoint Online utilizează limitarea pentru a menține performanța optimă și fiabilitatea serviciului SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="57276-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="57276-113">Limitarea limitează numărul de acțiuni ale utilizatorilor sau apeluri simultane (după script sau cod) pentru a preveni utilizarea exagerată a resurselor.</span><span class="sxs-lookup"><span data-stu-id="57276-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="57276-114">Pentru mai multe informații despre limitare, [consultați, Evitați să fiți sugrumat sau blocat în SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="57276-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="57276-115">Dacă credeți că această eroare nu are legătură cu limitarea, aveți posibilitatea să verificați dacă există întreținere activă care are loc pe entitategăzduită navigând la [centrul de mesaje](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="57276-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="57276-116">În cele din urmă, asigurați-vă că vizitați pagina [De sănătate a serviciilor](https://portal.office.com/adminportal/home#/servicehealth) pentru a verifica orice recomandări/incidente care pot apărea.</span><span class="sxs-lookup"><span data-stu-id="57276-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

