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
# <a name="restore-a-deleted-public-folder"></a>Restaurarea unui folder public șters

**Pentru a restaura elementele șterse dintr-un folder public**:

- Consultați [Nu puteți recupera elementele șterse dintr-un folder public non-mail în Outlook 2016](https://aka.ms/pfrec).
 
**Pentru a restaura un folder public șters (de orice tip)**: 

- Utilizați următoarea comandă EXO PowerShell:

    Sintaxa:

    >$pf=Ia-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Nume -eq\<" name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity \<-Calea cale în cazul în care folderul va fi restaurat>

    Exemplu: Următoarea comandă va restaura Subfolder1 și o va plasa sub \Parent1:

    >$pf=Ia-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Nume -eq "Subfolder1"}; Set-PublicFolder $pf.identity -Calea \Parent1

Consultați [Restaurarea unui folder public șters](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) pentru mai multe detalii.
