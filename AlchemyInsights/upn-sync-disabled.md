---
title: Sincronizare UPN dezactivată
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726116"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="90fbb-102">Sincronizare UPN dezactivată</span><span class="sxs-lookup"><span data-stu-id="90fbb-102">UPN sync disabled</span></span>

<span data-ttu-id="90fbb-103">Dacă ați început sincronizarea cu Azure AD înainte de 30 martie 2016, executați următorul cmdlet Azure AD PowerShell pentru a activa upn soft match pentru organizația dvs.:</span><span class="sxs-lookup"><span data-stu-id="90fbb-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="90fbb-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="90fbb-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="90fbb-105">Upn soft match este activat automat pentru organizațiile care au început sincronizarea cu Azure AD pe sau după 30 martie 2016.</span><span class="sxs-lookup"><span data-stu-id="90fbb-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="90fbb-106">Pentru a afla mai multe despre activarea potrivirii soft pe UPN și alte caracteristici de sincronizare, consultați [caracteristicile serviciului de sincronizare Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="90fbb-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

