---
title: Sharing cu utilizatorii externi nu este de lucru
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
ms.openlocfilehash: 700e6d24e49cf11bf91780895f5a796cc1d8349d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753438"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="9131b-102">Remediați problemele conținut SharePoint de partajare cu utilizatorii externi</span><span class="sxs-lookup"><span data-stu-id="9131b-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="9131b-103">Asiguraţi-vă că partajarea externă este activată pentru organizaţie:</span><span class="sxs-lookup"><span data-stu-id="9131b-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="9131b-104">Du-te la [servicii &amp; pagina de completare în centrul de administrare Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), faceţi clic pe **site-uri**.</span><span class="sxs-lookup"><span data-stu-id="9131b-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="9131b-105">Asiguraţi-vă că setarea este apelat la "Pe".</span><span class="sxs-lookup"><span data-stu-id="9131b-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="9131b-106">Dacă este selectat "Doar utilizatorii existenţi externe", asiguraţi-vă că utilizatorul extern este listat în centrul de administrare Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9131b-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="9131b-107">Asiguraţi-vă că extern de partajare-l activat pentru site-ul.</span><span class="sxs-lookup"><span data-stu-id="9131b-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="9131b-108">Pentru o colecţie de site-ul clasic:</span><span class="sxs-lookup"><span data-stu-id="9131b-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="9131b-109">În centrul de administrare SharePoint clasic, în panoul din stânga, faceţi clic pe **site-ul colecţii**.</span><span class="sxs-lookup"><span data-stu-id="9131b-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="9131b-110">Selectaţi site-ul sau site-uri, şi panglică, faceţi clic pe **Partajare**.</span><span class="sxs-lookup"><span data-stu-id="9131b-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="9131b-111">Pentru un site de echipă, care aparţine unui grup de Office 365, sau un site de comunicare:</span><span class="sxs-lookup"><span data-stu-id="9131b-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="9131b-112">Aceste tipuri de site-ul nou au setarea partajare aceeaşi ca setarea de nivel de organizaţie, dacă setarea de nivel de organizaţie permite partajarea fişierelor folosind link-uri care nu necesită autentificare.</span><span class="sxs-lookup"><span data-stu-id="9131b-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="9131b-113">În acest caz, site-uri permite partajarea cu noi și existente de utilizatori externi care semnează în.</span><span class="sxs-lookup"><span data-stu-id="9131b-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="9131b-114">Pentru a modifica setarea pentru anumite site-uri, utilizaţi noul centru de administrare SharePoint (preview) sau PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9131b-114">To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell.</span></span> <span data-ttu-id="9131b-115">[Aflaţi mai multe](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="9131b-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="9131b-116">Setarea de partajare externă pentru orice site poate fi mai restrictive decât setarea de nivel de organizaţie, dar nu mai permisivă decât setarea de nivel de organizaţie.</span><span class="sxs-lookup"><span data-stu-id="9131b-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

