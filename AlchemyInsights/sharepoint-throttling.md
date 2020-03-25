---
title: Limitare sharepoint online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931454"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="f1e54-102">Limitare sharepoint online</span><span class="sxs-lookup"><span data-stu-id="f1e54-102">SharePoint Online throttling</span></span>

<span data-ttu-id="f1e54-103">**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal.</span><span class="sxs-lookup"><span data-stu-id="f1e54-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f1e54-104">Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă.</span><span class="sxs-lookup"><span data-stu-id="f1e54-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f1e54-105">În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.</span><span class="sxs-lookup"><span data-stu-id="f1e54-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f1e54-106">În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii.</span><span class="sxs-lookup"><span data-stu-id="f1e54-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f1e54-107">Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade.</span><span class="sxs-lookup"><span data-stu-id="f1e54-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f1e54-108">Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.</span><span class="sxs-lookup"><span data-stu-id="f1e54-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f1e54-109">**Limitare sharepoint online**</span><span class="sxs-lookup"><span data-stu-id="f1e54-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="f1e54-110">SharePoint Online utilizează limitarea pentru a menține performanța optimă și fiabilitatea serviciului SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="f1e54-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="f1e54-111">Limitarea limitează numărul de acțiuni ale utilizatorilor sau apeluri simultane (după script sau cod) pentru a preveni utilizarea exagerată a resurselor.</span><span class="sxs-lookup"><span data-stu-id="f1e54-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="f1e54-112">Pentru mai multe informații, vă rugăm să vizitați link-urile de mai jos.</span><span class="sxs-lookup"><span data-stu-id="f1e54-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="f1e54-113">Evitați să fiți sugrumat sau blocat în SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f1e54-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="f1e54-114">Migrarea datelor și limitarea SPO</span><span class="sxs-lookup"><span data-stu-id="f1e54-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="f1e54-115">Viteza migrării SharePoint Online și OneDrive</span><span class="sxs-lookup"><span data-stu-id="f1e54-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="f1e54-116">Gestionați limitarea SharePoint Online utilizând înapoi exponențial</span><span class="sxs-lookup"><span data-stu-id="f1e54-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="f1e54-117">Planificarea capacităților și testarea sarcinii SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f1e54-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

