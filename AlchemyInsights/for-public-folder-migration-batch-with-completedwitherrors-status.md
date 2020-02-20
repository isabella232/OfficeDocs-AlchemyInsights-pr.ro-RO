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
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158630"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Pentru public folder migrare batch cu CompletedWithErrors stare

Utilizați următorii pași pentru a finaliza lotul, sărind peste elementele mari/nere: 
1. Aprobați elementele ignorate din grupul de migrare:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Utilizați următoarea comandă pentru a aproba elementele ignorate la solicitările de migrare care sunt "sincronizate", dar nu s-au terminat:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Lotul de migrare și solicitările ar trebui să reia și să se finalizeze în câteva minute.

