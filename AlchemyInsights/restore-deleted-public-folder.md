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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943387"
---
# <a name="restore-a-deleted-public-folder"></a>Restaurarea unui folder public șters

**Pentru a restaura elementele șterse dintr-un folder public:**

- Consultați [Nu puteți recupera elemente șterse dintr-un folder public non-mail din Outlook 2016](https://aka.ms/pfrec).
 
**Pentru a restaura un folder public șters (de orice tip)**: 

- Utilizați următoarea comandă EXO PowerShell:

    Sintaxă:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Exemplu: Următoarea comandă va restaura Subfolder1 și o va plasa sub \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Pentru [mai multe detalii, consultați Restaurarea unui folder public](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) șters.
