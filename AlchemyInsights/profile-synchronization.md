---
title: Sincronizare profil
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320721"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Când se sincronizează modificările profilului meu cu SharePoint Profil utilizator?

SharePoint Online utilizează activitatea de importare a timpului Active Directory (Import AD) pentru a importa utilizatori și grupuri în Aplicația profil utilizator. 
  
1. AD Import sincronizează modificările din SharePoint Online Directory Store în Aplicația profil utilizator. Aceste modificări sunt procesate în loturi.
    
2. Activitate de timer rulează până când se sincronizează modificările.
    
**Notă:** Timpul necesar pentru rularea funcției depinde de numărul de modificări de procesat. Un număr mare de modificări durează mai mult. Acordul la nivel de serviciu (SLA) spune că o modificare a unui utilizator din directorul SharePoint Online se va reflecta în Aplicația profil utilizator în 24 de ore. 
  
[Mai multe informații despre sincronizarea profilului de utilizator în SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

