---
title: Servicii de acces la pensie
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747796"
---
# <a name="access-services-retirement"></a><span data-ttu-id="8227b-102">Servicii de acces la pensie</span><span class="sxs-lookup"><span data-stu-id="8227b-102">Access services retirement</span></span>

<span data-ttu-id="8227b-103">Așa am anunțat inițial în MC97576, în martie 2017, și a continuat să comunice pe parcursul anului trecut servicii de acces sunt fiind retras din Office 365.</span><span class="sxs-lookup"><span data-stu-id="8227b-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="8227b-104">Următoarea fază din acest proces va fi eliminarea bazelor de date Access web care utilizează liste SharePoint ca stocarea datelor subiacente.</span><span class="sxs-lookup"><span data-stu-id="8227b-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="8227b-105">**mă afectează asta?**</span><span class="sxs-lookup"><span data-stu-id="8227b-105">**How does this affect me?**</span></span>

<span data-ttu-id="8227b-106">Începând cu iunie 2019, vom opri crearea de noi baze de date Access în SharePoint Online și închideți serviciul și orice aplicații rămase până în aprilie 2020.</span><span class="sxs-lookup"><span data-stu-id="8227b-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="8227b-107">**Ce trebuie să fac pentru a mă pregăti pentru această schimbare?**</span><span class="sxs-lookup"><span data-stu-id="8227b-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="8227b-108">Vă încurajăm să creați un plan de tranziție pentru bazele de date Web Access ale organizației dvs.</span><span class="sxs-lookup"><span data-stu-id="8227b-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="8227b-109">Administratorii pot utiliza [scanerul aplicației SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) pentru a obține un inventar al aplicațiilor Access pe care le utilizează site-urile.</span><span class="sxs-lookup"><span data-stu-id="8227b-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="8227b-110">Există mai multe modalități de a migra datele de baze de date Web Access:</span><span class="sxs-lookup"><span data-stu-id="8227b-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="8227b-111">Importul într-o bază de date Access locală (. ACCDB) sau într-un fișier Excel.</span><span class="sxs-lookup"><span data-stu-id="8227b-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="8227b-112">De asemenea, recomandăm explorarea Microsoft PowerApps ca o platformă alternativă pentru a crea soluții de afaceri fără cod pentru dispozitive web și mobile.</span><span class="sxs-lookup"><span data-stu-id="8227b-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>