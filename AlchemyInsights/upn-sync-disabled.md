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
# <a name="upn-sync-disabled"></a><span data-ttu-id="2a35d-102">UPN sync cu handicap</span><span class="sxs-lookup"><span data-stu-id="2a35d-102">UPN sync disabled</span></span>

<span data-ttu-id="2a35d-103">În cazul în care aţi început sincronizarea la azuriu AD înainte de 30 martie 2016, executaţi cmdletul PowerShell de AD Azure următoarele pentru a permite UPN meci moale pentru organizaţie numai:</span><span class="sxs-lookup"><span data-stu-id="2a35d-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="2a35d-104">**Set-MsolDirSyncFeature-au EnableSoftMatchOnUpn-permite $True**</span><span class="sxs-lookup"><span data-stu-id="2a35d-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="2a35d-105">UPN moale meci automat este pornit pentru organizaţiile care începe sincronizarea la azuriu AD la sau după 30 martie 2016.</span><span class="sxs-lookup"><span data-stu-id="2a35d-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="2a35d-106">Pentru a afla mai multe despre activarea meci moale pe UPN şi alte caracteristici de sincronizare, vă rugăm să consultaţi [Azure AD conecta sync serviciu caracteristici](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="2a35d-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

