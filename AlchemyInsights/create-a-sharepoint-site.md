---
title: Crearea unui site SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ba682f3c2b2600031f6856621691b1e0fba64113
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786577"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="fe604-102">Crearea unui site SharePoint</span><span class="sxs-lookup"><span data-stu-id="fe604-102">Create a SharePoint site</span></span>

<span data-ttu-id="fe604-103">Creați sau gestionați site-uri de la [site-uri active](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) în centrul de administrare SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fe604-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="fe604-104">Pentru mai multe informații, consultați [gestionarea site-urilor din noul centru de administrare SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="fe604-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="fe604-105">Sfaturi</span><span class="sxs-lookup"><span data-stu-id="fe604-105">Tips:</span></span>

- <span data-ttu-id="fe604-106">**Nu** puteți crea un site cu aceeași adresă URL a unui site existent.</span><span class="sxs-lookup"><span data-stu-id="fe604-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="fe604-107">Dacă ați șters un site și doriți să reutilizați URL-ul, este posibil ca site-ul șters să existe încă sub [site-uri șterse](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="fe604-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="fe604-108">Site-ul va trebui să fie șters definitiv pentru a reutiliza adresa URL.</span><span class="sxs-lookup"><span data-stu-id="fe604-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="fe604-109">Pentru a elimina complet un site cu PowerShell, consultați exemplul cmdletului [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="fe604-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="fe604-110">Este posibil ca unii utilizatori să nu poată crea un site.</span><span class="sxs-lookup"><span data-stu-id="fe604-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="fe604-111">[Consultați Gestionarea creării site-urilor în SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="fe604-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="fe604-112">Este posibil ca site-ul să apară blocat la **crearea** mai lungă decât cea așteptată.</span><span class="sxs-lookup"><span data-stu-id="fe604-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="fe604-113">Dacă au trecut mai mult de 24 de ore de când ați văzut prima dată această problemă, vă rugăm să înregistrați un tichet de asistență.</span><span class="sxs-lookup"><span data-stu-id="fe604-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="fe604-114">În multe cazuri, lucrăm deja la o soluție.</span><span class="sxs-lookup"><span data-stu-id="fe604-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="fe604-115">Vă rugăm să ne dați cel puțin 24 de ore pentru a finaliza o soluție.</span><span class="sxs-lookup"><span data-stu-id="fe604-115">Please give us at least 24 hours to complete a solution.</span></span>
