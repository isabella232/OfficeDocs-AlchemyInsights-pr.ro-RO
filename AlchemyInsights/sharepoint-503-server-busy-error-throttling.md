---
title: Limitare online SharePoint
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751900"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="1d55d-102">Limitare online SharePoint</span><span class="sxs-lookup"><span data-stu-id="1d55d-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="1d55d-103">Utilizatorii pot primi un server 503 este ocupat de eroare atunci când încercați să navigați la site-uri SharePoint sau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1d55d-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="1d55d-104">Această eroare poate fi cauzată de limitare în cadrul serviciului SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1d55d-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="1d55d-105">SharePoint Online utilizează supraîncărcarea pentru a menține performanța optimă și fiabilitatea serviciului SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="1d55d-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="1d55d-106">Limitare limitează numărul de acțiuni de utilizator sau apeluri simultane (prin script sau cod) pentru a preveni utilizarea excesivă a resurselor.</span><span class="sxs-lookup"><span data-stu-id="1d55d-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="1d55d-107">Dacă nu te Throttled, 99% din timp este din cauza codului personalizat.</span><span class="sxs-lookup"><span data-stu-id="1d55d-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="1d55d-108">Pentru mai multe informații despre limitare a se vedea, [evitați obtinerea limitate sau blocat în SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="1d55d-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="1d55d-109">Dacă credeți că această eroare nu are legătură cu supraîncărcarea, puteți verifica dacă există întreținere activă care apare pe entitate găzduită navigând la centrul de [mesaje](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="1d55d-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="1d55d-110">În cele din urmă, asigurați-vă că vizitați pagina de [sănătate a serviciului](https://portal.office.com/adminportal/home#/servicehealth) pentru a verifica pentru orice recomandări/incidente care pot fi apărute.</span><span class="sxs-lookup"><span data-stu-id="1d55d-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

