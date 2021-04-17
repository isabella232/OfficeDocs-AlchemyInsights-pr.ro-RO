---
title: Proprietarul nu poate crea sub folder utilizând Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836147"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Proprietarul nu poate crea sub folder utilizând Outlook

**Există o problemă continuă cu proprietarii de foldere publice, care creează subfoldere utilizând Outlook. Problema va fi remediată în curând.**

Între timp, utilizați una dintre următoarele soluții:

1. Utilizați Outlook pentru MAC pentru a crea subfolderul, deoarece problema afectează doar Outlook pentru ferestrele desktop (toate versiunile)
2. Spuneți administratorului să creeze subfolderul utilizând EXO Shell sau EAC
3. Modificați DefaultPublicFolderMailbox/EffectivePublicFolderMailbox a utilizatorului la altă cutie poștală decât cutia poștală de conținut, pentru folderul care provoacă problema  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Așteptați o oră, reporniți clientul Outlook