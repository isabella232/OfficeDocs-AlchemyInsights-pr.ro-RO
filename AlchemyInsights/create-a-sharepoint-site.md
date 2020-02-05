---
title: Crearea unui site SharePoint
ms.author: pebaum
author: todmccoy
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
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770867"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="a5e30-102">Crearea unui site SharePoint</span><span class="sxs-lookup"><span data-stu-id="a5e30-102">Create a SharePoint site</span></span>

<span data-ttu-id="a5e30-103">Creați sau gestionați site-uri din [Site-uri active](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) din Centrul de administrare SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5e30-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="a5e30-104">Pentru mai multe informații, consultați [Gestionarea site-urilor în noul centru de administrare SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="a5e30-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="a5e30-105">Sfaturi:</span><span class="sxs-lookup"><span data-stu-id="a5e30-105">Tips:</span></span>

- <span data-ttu-id="a5e30-106">Imposibil **de** creat un site cu același URL al unui site existent.</span><span class="sxs-lookup"><span data-stu-id="a5e30-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="a5e30-107">Dacă ați șters un site și doriți să reutilizați URL-ul, este posibil ca site-ul șters să existe în continuare sub [Site-uri șterse](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="a5e30-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="a5e30-108">Site-ul va trebui să fie șters definitiv pentru a reutiliza URL-ul.</span><span class="sxs-lookup"><span data-stu-id="a5e30-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="a5e30-109">Pentru a elimina complet un site cu Powershell, consultați exemplul cmdletului [Remove-SPSite.](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="a5e30-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="a5e30-110">Este posibil ca unii utilizatori să nu poată crea un site.</span><span class="sxs-lookup"><span data-stu-id="a5e30-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="a5e30-111">[Consultați Gestionarea creării de site-uri în SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="a5e30-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="a5e30-112">Este posibil ca site-ul să apară blocat la **Crearea** mai mult decât se aștepta.</span><span class="sxs-lookup"><span data-stu-id="a5e30-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="a5e30-113">Dacă au trecut mai mult de 24 de ore de când ați văzut prima dată această problemă, vă rugăm să vă conectați un bilet de asistență.</span><span class="sxs-lookup"><span data-stu-id="a5e30-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="a5e30-114">În multe cazuri, lucrăm deja la o soluție.</span><span class="sxs-lookup"><span data-stu-id="a5e30-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="a5e30-115">Vă rugăm să ne dea cel puțin 24 de ore pentru a finaliza o soluție.</span><span class="sxs-lookup"><span data-stu-id="a5e30-115">Please give us at least 24 hours to complete a solution.</span></span>
