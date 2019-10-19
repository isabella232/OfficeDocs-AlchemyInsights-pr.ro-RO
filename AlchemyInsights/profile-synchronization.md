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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Când se modifică profilul meu sincronizarea la aplicația profil de utilizator SharePoint?

SharePoint Online utilizează serviciul de cronometrare Active Directory import (AD import) pentru a importa utilizatori și grupuri în aplicația profil utilizator. 
  
1. AD Import sincronizează modificările din SharePoint Online Directory Store la aplicația profil utilizator. Aceste modificări sunt procesate în loturi.
    
2. Activitatea de cronometrare se execută până când modificările sunt sincronizate.
    
> [!NOTE]
> Timpul necesar pentru executarea lucrării depinde de numărul modificărilor de procesat. Un număr mare de modificări durează mai mult. Serviciul nivel acord (SLA) afirmă că o modificare a unui utilizator în SharePoint Online Directory se va reflecta în aplicația profil utilizator în 24 de ore. 
  
[Mai multe informații despre sincronizarea profilului de utilizator în SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

