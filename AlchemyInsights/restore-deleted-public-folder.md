---
title: Restaurarea unui folder public șters
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809451"
---
# <a name="restore-a-deleted-public-folder"></a>Restaurarea unui folder public șters

**Pentru a restaura elementele șterse dintr-un folder public:**

- Consultați [Nu puteți recupera elemente șterse dintr-un folder public non-mail din Outlook 2016.](https://aka.ms/pfrec)
 
**Pentru a restaura un folder public șters (de orice tip)**: 

- Utilizați următoarea comandă EXO PowerShell:

    Sintaxă:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Exemplu: Următoarea comandă va restaura Subfolder1 și o va plasa sub \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Pentru [mai multe detalii, consultați Restaurarea unui folder public](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) șters.
