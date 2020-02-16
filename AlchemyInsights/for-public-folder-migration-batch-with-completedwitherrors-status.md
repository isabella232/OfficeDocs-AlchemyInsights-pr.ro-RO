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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Pentru public folder migrare batch cu CompletedWithErrors stare

Utilizați următorii pași pentru a finaliza lotul, sărind peste elementele mari/nere: 
1. Aprobați elementele ignorate din grupul de migrare:

    Set-MigrationBatch \<batchname> -ApproveSkippedItems 
2. Utilizați următoarea comandă pentru a aproba elementele ignorate la solicitările de migrare care sunt "sincronizate", dar nu s-au terminat:

    $pf=Ia-PublicFolderMailboxMigrationRequest | Obțineți-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i în $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}
3. Lotul de migrare și solicitările ar trebui să reia și să se finalizeze în câteva minute.

