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
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063724"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="61929-102">Restaurarea unui folder public șters</span><span class="sxs-lookup"><span data-stu-id="61929-102">Restore a deleted public folder</span></span>

<span data-ttu-id="61929-103">**Pentru a restaura elementele șterse dintr-un folder public**:</span><span class="sxs-lookup"><span data-stu-id="61929-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="61929-104">Consultați [Nu puteți recupera elementele șterse dintr-un folder public non-mail în Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="61929-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="61929-105">**Pentru a restaura un folder public șters (de orice tip)**:</span><span class="sxs-lookup"><span data-stu-id="61929-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="61929-106">Utilizați următoarea comandă EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="61929-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="61929-107">Sintaxa:</span><span class="sxs-lookup"><span data-stu-id="61929-107">Syntax:</span></span>

    ><span data-ttu-id="61929-108">$pf=Ia-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Nume -eq\<" name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity \<-Calea cale în cazul în care folderul va fi restaurat></span><span class="sxs-lookup"><span data-stu-id="61929-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="61929-109">Exemplu: Următoarea comandă va restaura Subfolder1 și o va plasa sub \Parent1:</span><span class="sxs-lookup"><span data-stu-id="61929-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="61929-110">$pf=Ia-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Nume -eq "Subfolder1"}; Set-PublicFolder $pf.identity -Calea \Parent1</span><span class="sxs-lookup"><span data-stu-id="61929-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="61929-111">Consultați [Restaurarea unui folder public șters](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="61929-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
