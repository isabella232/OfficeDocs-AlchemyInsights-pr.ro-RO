---
title: Restaurarea unui folder public șters
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158534"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="984e6-102">Restaurarea unui folder public șters</span><span class="sxs-lookup"><span data-stu-id="984e6-102">Restore a deleted public folder</span></span>

<span data-ttu-id="984e6-103">**Pentru a restaura elementele șterse dintr-un folder public**:</span><span class="sxs-lookup"><span data-stu-id="984e6-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="984e6-104">Consultați [Nu puteți recupera elementele șterse dintr-un folder public non-mail în Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="984e6-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="984e6-105">**Pentru a restaura un folder public șters (de orice tip)**:</span><span class="sxs-lookup"><span data-stu-id="984e6-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="984e6-106">Utilizați următoarea comandă EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="984e6-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="984e6-107">Sintaxa:</span><span class="sxs-lookup"><span data-stu-id="984e6-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="984e6-108">Exemplu: Următoarea comandă va restaura Subfolder1 și o va plasa sub \Parent1:</span><span class="sxs-lookup"><span data-stu-id="984e6-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="984e6-109">Consultați [Restaurarea unui folder public șters](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="984e6-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
