---
title: Migrarea opțiunilor la SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932742"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="9ee13-102">Migrarea opțiunilor la SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9ee13-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="9ee13-103">**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal.</span><span class="sxs-lookup"><span data-stu-id="9ee13-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="9ee13-104">Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă.</span><span class="sxs-lookup"><span data-stu-id="9ee13-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="9ee13-105">În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.</span><span class="sxs-lookup"><span data-stu-id="9ee13-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="9ee13-106">În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii.</span><span class="sxs-lookup"><span data-stu-id="9ee13-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="9ee13-107">Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade.</span><span class="sxs-lookup"><span data-stu-id="9ee13-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="9ee13-108">Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.</span><span class="sxs-lookup"><span data-stu-id="9ee13-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="9ee13-109">**Opțiuni de migrare**</span><span class="sxs-lookup"><span data-stu-id="9ee13-109">**Migration options**</span></span>

<span data-ttu-id="9ee13-110">Există diferite opțiuni disponibile pentru migrarea conținutului în SharePoint Online, în funcție de dimensiunea și cantitatea de fișiere pe care trebuie să le mutați, consultați o listă de opțiuni [situate aici](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="9ee13-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="9ee13-111">Pentru mai multe informații despre migrarea conținutului, vizitați linkurile de mai jos.</span><span class="sxs-lookup"><span data-stu-id="9ee13-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="9ee13-112">Instrumentul de migrare Sharepoint</span><span class="sxs-lookup"><span data-stu-id="9ee13-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="9ee13-113">Introducere în Migration Manager</span><span class="sxs-lookup"><span data-stu-id="9ee13-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="9ee13-114">Viteza migrării Sharepoint Online și ODB</span><span class="sxs-lookup"><span data-stu-id="9ee13-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="9ee13-115">Evitați să fiți sugrumat sau blocat în SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9ee13-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="9ee13-116">Instrumentul de evaluare a migrării SharePoint (SMAT)</span><span class="sxs-lookup"><span data-stu-id="9ee13-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="9ee13-117">**Notă:** În prezent, instrumentul de migrare SharePoint acceptă numai migrările din SharePoint 2010 și 2013.</span><span class="sxs-lookup"><span data-stu-id="9ee13-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="9ee13-118">Versiunea 2016 sau 2019 nu sunt acceptate în acest moment.</span><span class="sxs-lookup"><span data-stu-id="9ee13-118">Version 2016 or 2019 are not supported at this time.</span></span>
