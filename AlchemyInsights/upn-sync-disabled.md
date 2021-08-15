---
title: Sincronizarea UPN este dezactivată
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038124"
---
# <a name="upn-sync-disabled"></a>Sincronizarea UPN este dezactivată

Dacă a început să se sincronizeze cu Azure AD înainte de 30 martie 2016, rulați următorul cmdlet Azure AD PowerShell pentru a activa potrivirea soft UPN doar pentru organizația dvs.:
  
 **Set-MsolDirSyncFeature -Caracteristică EnableSoftMatchOnUpn -Activați $True**
  
UpN soft match este activat automat pentru organizațiile care au început să se sincronizeze cu Azure AD la sau după 30 martie 2016.
  
Pentru a afla mai multe despre activarea potrivirii virtuale în UPN și alte caracteristici de sincronizare, consultați [Azure AD Conectare caracteristicile serviciului de sincronizare.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

