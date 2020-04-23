---
title: Sincronizare profil
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768125"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="e75fd-102">Când se modifică profilul meu în aplicația Profil utilizator SharePoint?</span><span class="sxs-lookup"><span data-stu-id="e75fd-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="e75fd-103">SharePoint Online utilizează activitatea de cronometrare Import Active Directory (Import AD) pentru a importa utilizatori și grupuri în aplicația profil utilizator.</span><span class="sxs-lookup"><span data-stu-id="e75fd-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="e75fd-104">AD Import sincronizează modificările din Depozitul de director SharePoint Online la aplicația profil utilizator.</span><span class="sxs-lookup"><span data-stu-id="e75fd-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="e75fd-105">Aceste modificări sunt procesate în loturi.</span><span class="sxs-lookup"><span data-stu-id="e75fd-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="e75fd-106">Activitatea cronometru se execută până când modificările sunt sincronizate.</span><span class="sxs-lookup"><span data-stu-id="e75fd-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="e75fd-107">Timpul necesar pentru executarea lucrării depinde de numărul de modificări ale procesului.</span><span class="sxs-lookup"><span data-stu-id="e75fd-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="e75fd-108">Un număr mare de modificări durează mai mult.</span><span class="sxs-lookup"><span data-stu-id="e75fd-108">A large number of changes takes longer.</span></span> <span data-ttu-id="e75fd-109">Acordul de nivel de serviciu (SLA) afirmă că o modificare a unui utilizator în Directorul SharePoint Online se va reflecta în aplicația profil utilizator în 24 de ore.</span><span class="sxs-lookup"><span data-stu-id="e75fd-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="e75fd-110">Mai multe informații despre sincronizarea profilului de utilizator în SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="e75fd-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

