---
title: Sincronizarea profilului
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554345"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="3ffe3-102">Când se modifică profilul meu sincronizarea la aplicația profil de utilizator SharePoint?</span><span class="sxs-lookup"><span data-stu-id="3ffe3-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="3ffe3-103">SharePoint Online utilizează serviciul de cronometrare Active Directory import (AD import) pentru a importa utilizatori și grupuri în aplicația profil utilizator.</span><span class="sxs-lookup"><span data-stu-id="3ffe3-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="3ffe3-104">AD Import sincronizează modificările din SharePoint Online Directory Store la aplicația profil utilizator.</span><span class="sxs-lookup"><span data-stu-id="3ffe3-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="3ffe3-105">Aceste modificări sunt procesate în loturi.</span><span class="sxs-lookup"><span data-stu-id="3ffe3-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="3ffe3-106">Activitatea de cronometrare se execută până când modificările sunt sincronizate.</span><span class="sxs-lookup"><span data-stu-id="3ffe3-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="3ffe3-107">Timpul necesar pentru executarea lucrării depinde de numărul modificărilor de procesat.</span><span class="sxs-lookup"><span data-stu-id="3ffe3-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="3ffe3-108">Un număr mare de modificări durează mai mult.</span><span class="sxs-lookup"><span data-stu-id="3ffe3-108">A large number of changes takes longer.</span></span> <span data-ttu-id="3ffe3-109">Serviciul nivel acord (SLA) afirmă că o modificare a unui utilizator în SharePoint Online Directory se va reflecta în aplicația profil utilizator în 24 de ore.</span><span class="sxs-lookup"><span data-stu-id="3ffe3-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="3ffe3-110">Mai multe informații despre sincronizarea profilului de utilizator în SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="3ffe3-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

