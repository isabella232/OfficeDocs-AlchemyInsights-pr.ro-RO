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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Când se modifică profilul meu în aplicația Profil utilizator SharePoint?

SharePoint Online utilizează activitatea de cronometrare Import Active Directory (Import AD) pentru a importa utilizatori și grupuri în aplicația profil utilizator. 
  
1. AD Import sincronizează modificările din Depozitul de director SharePoint Online la aplicația profil utilizator. Aceste modificări sunt procesate în loturi.
    
2. Activitatea cronometru se execută până când modificările sunt sincronizate.
    
> [!NOTE]
> Timpul necesar pentru executarea lucrării depinde de numărul de modificări ale procesului. Un număr mare de modificări durează mai mult. Acordul de nivel de serviciu (SLA) afirmă că o modificare a unui utilizator în Directorul SharePoint Online se va reflecta în aplicația profil utilizator în 24 de ore. 
  
[Mai multe informații despre sincronizarea profilului de utilizator în SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

