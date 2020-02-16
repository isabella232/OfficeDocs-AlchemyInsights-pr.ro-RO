---
title: Pentru public folder migrare batch cu CompletedWithErrors stare
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
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043611"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="c67c5-102">Pentru public folder migrare batch cu CompletedWithErrors stare</span><span class="sxs-lookup"><span data-stu-id="c67c5-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="c67c5-103">Utilizați următorii pași pentru a finaliza lotul, sărind peste elementele mari/nere:</span><span class="sxs-lookup"><span data-stu-id="c67c5-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="c67c5-104">Aprobați elementele ignorate din grupul de migrare:</span><span class="sxs-lookup"><span data-stu-id="c67c5-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="c67c5-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span><span class="sxs-lookup"><span data-stu-id="c67c5-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="c67c5-106">Utilizați următoarea comandă pentru a aproba elementele ignorate la solicitările de migrare care sunt "sincronizate", dar nu s-au terminat:</span><span class="sxs-lookup"><span data-stu-id="c67c5-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="c67c5-107">$pf=Ia-PublicFolderMailboxMigrationRequest | Obțineți-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i în $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}</span><span class="sxs-lookup"><span data-stu-id="c67c5-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="c67c5-108">Lotul de migrare și solicitările ar trebui să reia și să se finalizeze în câteva minute.</span><span class="sxs-lookup"><span data-stu-id="c67c5-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

