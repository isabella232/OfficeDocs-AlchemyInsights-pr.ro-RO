---
title: Sincronizare UPN dezactivată
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749526"
---
# <a name="upn-sync-disabled"></a>Sincronizare UPN dezactivată

Dacă ați început sincronizarea la Azure AD înainte de 30 martie, 2016, rulează următorul cmdlet Azure AD PowerShell pentru a activa UPN soft Match doar pentru organizația dvs.:
  
 **Set-MsolDirSyncFeature-feature EnableSoftMatchOnUpn-Enable $True**
  
Meciul cu UPN soft este activat automat pentru organizațiile care au început sincronizarea la Azure AD la sau după 30 martie 2016.
  
Pentru a afla mai multe despre activarea soft Match pe UPN și alte caracteristici de sincronizare, consultați [caracteristici de serviciu de sincronizare AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

