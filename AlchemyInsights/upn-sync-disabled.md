---
title: UPN sync cu handicap
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29485260"
---
# <a name="upn-sync-disabled"></a>UPN sync cu handicap

În cazul în care aţi început sincronizarea la azuriu AD înainte de 30 martie 2016, executaţi cmdletul PowerShell de AD Azure următoarele pentru a permite UPN meci moale pentru organizaţie numai:
  
 **Set-MsolDirSyncFeature-au EnableSoftMatchOnUpn-permite $True**
  
UPN moale meci automat este pornit pentru organizaţiile care începe sincronizarea la azuriu AD la sau după 30 martie 2016.
  
Pentru a afla mai multe despre activarea meci moale pe UPN şi alte caracteristici de sincronizare, vă rugăm să consultaţi [Azure AD conecta sync serviciu caracteristici](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

