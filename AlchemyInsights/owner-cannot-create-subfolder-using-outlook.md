---
title: Proprietarul nu poate crea subfolder utilizând Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665730"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Proprietarul nu poate crea subfolder utilizând Outlook

**Există o problemă în curs de desfășurare cu proprietarii de foldere publice care creează subfoldere utilizând Outlook. Problema va fi remediată în curând.**

Între timp, utilizați una dintre următoarele soluții:

1. Utilizați Outlook pentru MAC pentru a crea subfolderul ca problema afectează numai Outlook pentru desktop Windows (toate versiunile)
2. Administratorul să creeze subfolderul utilizând EXO Shell sau EAC
3. Modificarea DefaultPublicFolderMailbox/EffectivePublicFolderMailbox pentru utilizator în altă cutie poștală decât cutia poștală de conținut pentru folderul care cauzează problema  
    - *Set-cutia poștală user1 DefaultPublicFolderMailbox PubMBX3*
4. Așteptați o oră, reporniți clientul Outlook