---
title: Limitare SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773859"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="c3d42-102">Limitare SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c3d42-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="c3d42-103">**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="c3d42-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c3d42-104">**eroarea Server 503 este ocupată**</span><span class="sxs-lookup"><span data-stu-id="c3d42-104">**503 server is busy error**</span></span>

<span data-ttu-id="c3d42-105">Utilizatorii pot primi un server 503 este o eroare ocupată atunci când încercați să navigați la site-uri SharePoint sau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c3d42-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="c3d42-106">Această eroare poate fi cauzată de limitarea în serviciul SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c3d42-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="c3d42-107">SharePoint Online utilizează limitarea pentru a menține performanța optimă și fiabilitatea serviciului SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c3d42-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="c3d42-108">Limitarea se aplică la numărul de acțiuni de utilizator sau apeluri concurente (după script sau cod), pentru a preveni utilizarea excesivă a resurselor.</span><span class="sxs-lookup"><span data-stu-id="c3d42-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="c3d42-109">Pentru mai multe informații despre limitare, consultați [evitați să fiți accelerat sau blocat în SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="c3d42-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="c3d42-110">Dacă credeți că această eroare nu are legătură cu limitarea, puteți să verificați dacă există întreținere activă care apare în entitatea găzduită, navigând la [Centrul de mesaje](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="c3d42-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="c3d42-111">În cele din urmă, asigurați-vă că vizitați pagina stare [servicii](https://portal.office.com/adminportal/home#/servicehealth) pentru a verifica dacă există recomandări/incidente care pot apărea.</span><span class="sxs-lookup"><span data-stu-id="c3d42-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

