---
title: Acces la servicii de pensionare
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 5f171050479f34077f3dc155bec40437f86b84c0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35359371"
---
# <a name="access-services-retirement"></a><span data-ttu-id="b41ef-102">Acces la servicii de pensionare</span><span class="sxs-lookup"><span data-stu-id="b41ef-102">Access services retirement</span></span>

<span data-ttu-id="b41ef-103">Aşa cum am anunţat în MC97576, în martie 2017, iniţial şi a continuat să comunice pe parcursul anului trecut serviciile de acces sunt fiind retras din Office 365.</span><span class="sxs-lookup"><span data-stu-id="b41ef-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="b41ef-104">Următoarea etapă în acest proces va fi eliminarea de acces Web baze de date care utilizează liste SharePoint ca depozitarea lor care stau la baza de date.</span><span class="sxs-lookup"><span data-stu-id="b41ef-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="b41ef-105">**Cum acest lucru afectează-mă?**</span><span class="sxs-lookup"><span data-stu-id="b41ef-105">**How does this affect me?**</span></span>

<span data-ttu-id="b41ef-106">Începând cu iunie 2019, vom opri crearea de baze de date Access nou în SharePoint Online şi opriţi serviciul şi orice apps rămase până în 2020, aprilie.</span><span class="sxs-lookup"><span data-stu-id="b41ef-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="b41ef-107">**Ce trebuie să fac pentru a se pregăti pentru această schimbare?**</span><span class="sxs-lookup"><span data-stu-id="b41ef-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="b41ef-108">Vă recomandăm să creaţi un plan de tranzitie pentru organizaţia dumneavoastră web de acces baze de date.</span><span class="sxs-lookup"><span data-stu-id="b41ef-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="b41ef-109">Administratori puteţi utiliza [SharePoint acces app scanerului](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) pentru a obţine un inventar de aplicaţii de acces care utilizează site-uri.</span><span class="sxs-lookup"><span data-stu-id="b41ef-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="b41ef-110">Există mai multe modalităţi de a migra datelor de baze de date acces web:</span><span class="sxs-lookup"><span data-stu-id="b41ef-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="b41ef-111">Importul unei baze de date Access local (. ACCDB) sau într-un fişier Excel.</span><span class="sxs-lookup"><span data-stu-id="b41ef-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="b41ef-112">De asemenea, recomandăm explorarea Microsoft PowerApps ca o platformă alternativă la crearea soluţiilor de no-codului pentru web şi dispozitive mobile.</span><span class="sxs-lookup"><span data-stu-id="b41ef-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>