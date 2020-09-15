---
title: Partajarea cu utilizatorii externi nu funcționează
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691587"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="61925-102">Remedierea problemelor cu partajarea conținutului SharePoint cu utilizatorii externi</span><span class="sxs-lookup"><span data-stu-id="61925-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="61925-103">Asigurați-vă că partajarea externă este activată pentru organizația dvs.:</span><span class="sxs-lookup"><span data-stu-id="61925-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="61925-104">Accesați pagina programe [de &amp; completare servicii din centrul de administrare Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)și faceți clic pe **site-uri**.</span><span class="sxs-lookup"><span data-stu-id="61925-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="61925-105">Asigurați-vă că setarea este activată la "activat".</span><span class="sxs-lookup"><span data-stu-id="61925-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="61925-106">Dacă este selectat "doar utilizatori externi existenți", asigurați-vă că utilizatorul extern este listat în centrul de administrare Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="61925-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="61925-107">Asigurați-vă că ați activat partajarea externă pentru site.</span><span class="sxs-lookup"><span data-stu-id="61925-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="61925-108">Pentru o colecție de site-uri clasică:</span><span class="sxs-lookup"><span data-stu-id="61925-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="61925-109">În noul centru de administrare SharePoint, în panoul din stânga, faceți clic pe **site-uri**.</span><span class="sxs-lookup"><span data-stu-id="61925-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="61925-110">Selectați site-ul sau site-urile și, pe panglică, faceți clic pe **Partajare**.</span><span class="sxs-lookup"><span data-stu-id="61925-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="61925-111">Pentru un site de echipă care aparține unui grup Microsoft 365 sau unui site de comunicare:</span><span class="sxs-lookup"><span data-stu-id="61925-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="61925-112">Aceste tipuri noi de site-uri au aceeași setare de partajare ca și setarea la nivel de organizație, cu excepția cazului în care setarea la nivel de organizație permite partajarea fișierelor utilizând linkuri care nu necesită conectare.</span><span class="sxs-lookup"><span data-stu-id="61925-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="61925-113">În acest caz, site-urile permit partajarea cu utilizatori externi noi și existenți care se conectează.</span><span class="sxs-lookup"><span data-stu-id="61925-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="61925-114">Pentru a modifica setarea pentru anumite site-uri, utilizați noul centru de administrare SharePoint sau PowerShell.</span><span class="sxs-lookup"><span data-stu-id="61925-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="61925-115">[Aflați mai multe](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="61925-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="61925-116">Setarea de partajare externă pentru orice site poate fi mai restrictivă decât setarea la nivel de organizație, dar nu mai permisivă decât setarea la nivel de organizație.</span><span class="sxs-lookup"><span data-stu-id="61925-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

