---
title: Sincronizare profil
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29485654"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="9962d-102">Când sincronizează modificările de profil aplicația de profil utilizator SharePoint?</span><span class="sxs-lookup"><span data-stu-id="9962d-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="9962d-103">SharePoint Online foloseste Active Director Import cronometrare (AD Import) pentru a importa utilizatorii şi grupurile în aplicația de profil utilizator.</span><span class="sxs-lookup"><span data-stu-id="9962d-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="9962d-p101">AD Import se sincronizează modificările de la SharePoint Online Director magazin la aplicația de profil utilizator. Aceste modificări sunt prelucrate în loturi.</span><span class="sxs-lookup"><span data-stu-id="9962d-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="9962d-106">Cronometrare se execută până când modificările sunt sincronizate.</span><span class="sxs-lookup"><span data-stu-id="9962d-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="9962d-p102">Timpul este nevoie de locuri de muncă pentru a rula depinde de numărul de modificări pentru a procesa. Un număr mare de schimbări durează mai mult. Acord servicii de nivel (SLA) afirmă că o modificare a unui utilizator în SharePoint Online Director vor fi reflectate în aplicația de profil utilizator în 24 de ore.</span><span class="sxs-lookup"><span data-stu-id="9962d-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="9962d-110">Mai multe informaţii despre sincronizarea profilului de utilizator în SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9962d-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

