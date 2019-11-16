---
title: Restaurarea unui site șters
ms.author: kaarins
author: kaarins
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: a1fb15869b9f576696de4eda4c0b2101bd6cca17
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768560"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="4d9db-102">Restaurarea unui site șters</span><span class="sxs-lookup"><span data-stu-id="4d9db-102">Restore a deleted site</span></span>

<span data-ttu-id="4d9db-103">Atunci când un administrator șterge un site SharePoint, este plasat în colecția de site-ul de reciclare coșul, unde este păstrat pentru 93 zile înainte de a fi șters definitiv.</span><span class="sxs-lookup"><span data-stu-id="4d9db-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="4d9db-104">Pentru a restaura site-ul:</span><span class="sxs-lookup"><span data-stu-id="4d9db-104">To restore the site:</span></span>
  
1. <span data-ttu-id="4d9db-105">În noul centru de administrare SharePoint, faceți clic pe **Coșul de reciclare** din panglică.</span><span class="sxs-lookup"><span data-stu-id="4d9db-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="4d9db-106">Bifați caseta de selectare de lângă colecția de site-uri pe care doriți să o restaurați.</span><span class="sxs-lookup"><span data-stu-id="4d9db-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="4d9db-107">Faceți clic pe **Restaurare elemente șterse**.</span><span class="sxs-lookup"><span data-stu-id="4d9db-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="4d9db-108">Pentru a restaura un site de comunicare șters, aveți posibilitatea să utilizați noul centru de administrare SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4d9db-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="4d9db-109">În caz contrar, trebuie să utilizați Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4d9db-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="4d9db-110">Pentru a restaura un site care aparține unui grup Office 365, trebuie să restaurați grupul în centrul de administrare Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d9db-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="4d9db-111">Grupurile pot fi restaurate timp de 30 de zile după ce sunt șterse.</span><span class="sxs-lookup"><span data-stu-id="4d9db-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

