---
title: Restaurarea unui folder public șters
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774543"
---
# <a name="restore-a-deleted-public-folder"></a>Restaurarea unui folder public șters

**Pentru a restaura elementele șterse dintr-un folder public**:

- Consultați [nu puteți recupera elementele șterse dintr-un folder public non-corespondență din Outlook 2016](https://aka.ms/pfrec).
 
**Pentru a restaura un folder public șters (de orice tip)**: 

- Vă rugăm să utilizați următoarea comandă EXO PowerShell:

    Sintaxa

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Exemplu: următoarea comandă va restabili Subfolder1 și o plasează sub \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Consultați [restaurarea unui folder public șters](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) pentru mai multe detalii.
