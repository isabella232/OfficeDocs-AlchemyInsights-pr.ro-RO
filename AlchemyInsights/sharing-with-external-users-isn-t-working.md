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
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502243"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="f3964-102">Remediați problemele conținut SharePoint de partajare cu utilizatorii externi</span><span class="sxs-lookup"><span data-stu-id="f3964-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="f3964-103">Asiguraţi-vă că partajarea externă este activată pentru organizaţie:</span><span class="sxs-lookup"><span data-stu-id="f3964-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="f3964-104">Du-te la [servicii &amp; pagina de completare în centrul de administrare Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), faceţi clic pe **site-uri**.</span><span class="sxs-lookup"><span data-stu-id="f3964-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="f3964-105">Asiguraţi-vă că setarea este apelat la "Pe".</span><span class="sxs-lookup"><span data-stu-id="f3964-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="f3964-106">Dacă este selectat "Doar utilizatorii existenţi externe", asiguraţi-vă că utilizatorul extern este listat în centrul de administrare Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f3964-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="f3964-107">Asiguraţi-vă că extern de partajare-l activat pentru site-ul.</span><span class="sxs-lookup"><span data-stu-id="f3964-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="f3964-108">Pentru o colecţie de site-ul clasic:</span><span class="sxs-lookup"><span data-stu-id="f3964-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="f3964-109">În noul centru de administrare SharePoint, în panoul din stânga, faceţi clic pe **site-uri**.</span><span class="sxs-lookup"><span data-stu-id="f3964-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="f3964-110">Selectaţi site-ul sau site-uri, şi panglică, faceţi clic pe **Partajare**.</span><span class="sxs-lookup"><span data-stu-id="f3964-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="f3964-111">Pentru un site de echipă, care aparţine unui grup de Office 365, sau un site de comunicare:</span><span class="sxs-lookup"><span data-stu-id="f3964-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="f3964-112">Aceste tipuri de site-ul nou au setarea partajare aceeaşi ca setarea de nivel de organizaţie, dacă setarea de nivel de organizaţie permite partajarea fişierelor folosind link-uri care nu necesită autentificare.</span><span class="sxs-lookup"><span data-stu-id="f3964-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="f3964-113">În acest caz, site-uri permite partajarea cu noi și existente de utilizatori externi care semnează în.</span><span class="sxs-lookup"><span data-stu-id="f3964-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="f3964-114">Pentru a modifica setarea pentru anumite site-uri, utilizaţi centrul de administrare SharePoint noi sau PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f3964-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="f3964-115">[Aflaţi mai multe](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="f3964-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="f3964-116">Setarea de partajare externă pentru orice site poate fi mai restrictive decât setarea de nivel de organizaţie, dar nu mai permisivă decât setarea de nivel de organizaţie.</span><span class="sxs-lookup"><span data-stu-id="f3964-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

