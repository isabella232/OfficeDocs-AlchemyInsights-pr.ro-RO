---
title: Partajarea cu utilizatorii externi nu funcționează
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767261"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="4f849-102">Remedierea problemelor legate de partajarea conținutului SharePoint cu utilizatorii externi</span><span class="sxs-lookup"><span data-stu-id="4f849-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="4f849-103">Asigurați-vă că partajarea externă este activată pentru organizația dvs.:</span><span class="sxs-lookup"><span data-stu-id="4f849-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="4f849-104">Accesați [pagina &amp; Programe de completare Servicii din centrul de administrare Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)și faceți clic pe **Site-uri**.</span><span class="sxs-lookup"><span data-stu-id="4f849-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="4f849-105">Asigurați-vă că setarea este activată la "Activat".</span><span class="sxs-lookup"><span data-stu-id="4f849-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="4f849-106">Dacă este selectată opțiunea "Numai utilizatorii externi existenți", asigurați-vă că utilizatorul extern este listat în centrul de administrare Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4f849-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="4f849-107">Asigurați-vă că partajarea externă activată pentru site.</span><span class="sxs-lookup"><span data-stu-id="4f849-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="4f849-108">Pentru o colecție clasică de site-uri:</span><span class="sxs-lookup"><span data-stu-id="4f849-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="4f849-109">În noul centru de administrare SharePoint, în panoul din stânga, faceți clic pe **site-uri**.</span><span class="sxs-lookup"><span data-stu-id="4f849-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="4f849-110">Selectați site-ul sau site-urile, iar pe panglică, faceți clic pe **Partajare**.</span><span class="sxs-lookup"><span data-stu-id="4f849-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="4f849-111">Pentru un site de echipă care aparține unui grup Office 365 sau unui site de comunicare:</span><span class="sxs-lookup"><span data-stu-id="4f849-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="4f849-112">Aceste tipuri noi de site-uri au aceeași setare de partajare ca și setarea la nivel de organizație, cu excepția cazului în care setarea la nivel de organizație permite partajarea fișierelor utilizând linkuri care nu necesită conectare.</span><span class="sxs-lookup"><span data-stu-id="4f849-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="4f849-113">În acest caz, site-urile permit partajarea cu utilizatorii externi noi și existenți care se conectează.</span><span class="sxs-lookup"><span data-stu-id="4f849-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="4f849-114">Pentru a modifica setarea pentru anumite site-uri, utilizați noul centru de administrare SharePoint sau PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4f849-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="4f849-115">[Aflați mai multe](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="4f849-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="4f849-116">Setarea de partajare externă pentru orice site poate fi mai restrictivă decât setarea la nivel de organizație, dar nu mai permisivă decât setarea la nivel de organizație.</span><span class="sxs-lookup"><span data-stu-id="4f849-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

