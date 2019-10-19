---
title: Partajarea cu utilizatorii externi nu funcționează
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502243"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="50f16-102">Remedierea problemelor cu partajarea conținutului SharePoint cu utilizatorii externi</span><span class="sxs-lookup"><span data-stu-id="50f16-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="50f16-103">Asigurați-vă că partajarea externă este activată pentru organizația dvs.:</span><span class="sxs-lookup"><span data-stu-id="50f16-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="50f16-104">Accesați pagina de [ &amp; programe de completare din centrul de administrare Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)și faceți clic pe **site-uri**.</span><span class="sxs-lookup"><span data-stu-id="50f16-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="50f16-105">Asigurați-vă că setarea este activată "activat".</span><span class="sxs-lookup"><span data-stu-id="50f16-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="50f16-106">Dacă este selectată "numai utilizatorii externi existenți", asigurați-vă că utilizatorul extern este listat în centrul de administrare Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="50f16-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="50f16-107">Asigurați-vă că partajarea externă este activată pentru site.</span><span class="sxs-lookup"><span data-stu-id="50f16-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="50f16-108">Pentru o colecție de site-uri clasice:</span><span class="sxs-lookup"><span data-stu-id="50f16-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="50f16-109">În noul centru de administrare SharePoint, în panoul din stânga, faceți clic pe **site-uri**.</span><span class="sxs-lookup"><span data-stu-id="50f16-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="50f16-110">Selectați site-ul sau site-urile și, în panglică, faceți clic pe **Partajare**.</span><span class="sxs-lookup"><span data-stu-id="50f16-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="50f16-111">Pentru un site de echipă care aparține unui grup Office 365 sau un site de comunicare:</span><span class="sxs-lookup"><span data-stu-id="50f16-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="50f16-112">Aceste tipuri de site-uri noi au aceeași setare de partajare ca setarea la nivel de organizație, cu excepția cazului în care setarea la nivel de organizație permite partajarea fișierelor utilizând linkuri care nu necesită conectare.</span><span class="sxs-lookup"><span data-stu-id="50f16-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="50f16-113">În acest caz, site-urile permit partajarea cu utilizatori externi noi și existenți care se conectează.</span><span class="sxs-lookup"><span data-stu-id="50f16-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="50f16-114">Pentru a modifica setarea pentru anumite site-uri, utilizați noul centru de administrare SharePoint sau PowerShell.</span><span class="sxs-lookup"><span data-stu-id="50f16-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="50f16-115">[Aflați mai multe](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="50f16-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="50f16-116">Setarea de partajare externă pentru orice site poate fi mai restrictivă decât setarea la nivel de organizație, dar nu mai permisivă decât setarea la nivel de organizație.</span><span class="sxs-lookup"><span data-stu-id="50f16-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

