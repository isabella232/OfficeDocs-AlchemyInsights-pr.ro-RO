---
title: Retragere servicii Access
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698694"
---
# <a name="access-services-retirement"></a><span data-ttu-id="b74e6-102">Retragere servicii Access</span><span class="sxs-lookup"><span data-stu-id="b74e6-102">Access services retirement</span></span>

<span data-ttu-id="b74e6-103">Așa cum am anunțat inițial în MC97576, în martie 2017, și am continuat să comunicăm în ultimul an Access Services sunt retrase.</span><span class="sxs-lookup"><span data-stu-id="b74e6-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="b74e6-104">Următoarea etapă a acestui proces va fi eliminarea bazelor de date Web Access care utilizează liste SharePoint ca stocare de date subiacente.</span><span class="sxs-lookup"><span data-stu-id="b74e6-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="b74e6-105">**Cum mă afectează aceasta?**</span><span class="sxs-lookup"><span data-stu-id="b74e6-105">**How does this affect me?**</span></span>

<span data-ttu-id="b74e6-106">Începând cu luna iunie 2019, vom opri crearea de noi baze de date Access în SharePoint Online și vom închide serviciul și toate aplicațiile rămase până în aprilie 2020.</span><span class="sxs-lookup"><span data-stu-id="b74e6-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="b74e6-107">**Ce trebuie să fac pentru a mă pregăti pentru această modificare?**</span><span class="sxs-lookup"><span data-stu-id="b74e6-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="b74e6-108">Vă recomandăm să creați un plan de tranziție pentru bazele de date Web Access ale organizației dvs.</span><span class="sxs-lookup"><span data-stu-id="b74e6-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="b74e6-109">Administratorii pot utiliza [scanerul aplicației SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) pentru a obține un inventar al aplicațiilor Access pe care le utilizează site-urile.</span><span class="sxs-lookup"><span data-stu-id="b74e6-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="b74e6-110">Există mai multe modalități de a migra datele din bazele de date Web Access:</span><span class="sxs-lookup"><span data-stu-id="b74e6-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="b74e6-111">Importul într-o bază de date Access locală (. ACCDB) sau într-un fișier Excel.</span><span class="sxs-lookup"><span data-stu-id="b74e6-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="b74e6-112">De asemenea, recomandăm explorarea Microsoft PowerApps ca platformă alternativă pentru a crea soluții de Business fără cod pentru dispozitive web și mobile.</span><span class="sxs-lookup"><span data-stu-id="b74e6-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>