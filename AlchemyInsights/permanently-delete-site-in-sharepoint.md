---
title: Ștergerea definitivă a unui site din SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955241"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="18d6a-102">Ștergerea definitivă a unui site din SharePoint</span><span class="sxs-lookup"><span data-stu-id="18d6a-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="18d6a-103">Pentru a reutiliza un URL de pe un site șters (pentru a crea din nou un site) sau pentru a șterge definitiv un site deoarece nu mai este utilizat, puteți utiliza **Ștergere definitivă** din noul Centru de administrare SharePoint.</span><span class="sxs-lookup"><span data-stu-id="18d6a-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="18d6a-104">Accesați [pagina Site-uri șterse din noul centru de administrare SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) și conectați-vă cu un cont care are permisiuni de administrator pentru organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="18d6a-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="18d6a-105">Selectați un site din coloana din stânga.</span><span class="sxs-lookup"><span data-stu-id="18d6a-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="18d6a-106">Faceți clic pe **Ștergere definitivă**.</span><span class="sxs-lookup"><span data-stu-id="18d6a-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="18d6a-107">**Notă**: Site-urile conectate în grup nu pot fi șterse definitiv din noul Centru de administrare SharePoint.</span><span class="sxs-lookup"><span data-stu-id="18d6a-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="18d6a-108">În schimb, va trebui să utilizați [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).</span><span class="sxs-lookup"><span data-stu-id="18d6a-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="18d6a-109">Pentru mai multe informații, consultați [Ștergerea definită a unui site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="18d6a-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
