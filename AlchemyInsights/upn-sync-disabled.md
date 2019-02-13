---
title: UPN sync cu handicap
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921720"
---
# <a name="upn-sync-disabled"></a>UPN sync cu handicap

În cazul în care aţi început sincronizarea la azuriu AD înainte de 30 martie 2016, executaţi cmdletul PowerShell de AD Azure următoarele pentru a permite UPN meci moale pentru organizaţie numai:
  
 **Set-MsolDirSyncFeature-au EnableSoftMatchOnUpn-permite $True**
  
UPN moale meci automat este pornit pentru organizaţiile care începe sincronizarea la azuriu AD la sau după 30 martie 2016.
  
Pentru a afla mai multe despre activarea meci moale pe UPN şi alte caracteristici de sincronizare, vă rugăm să consultaţi [Azure AD conecta sync serviciu caracteristici](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

