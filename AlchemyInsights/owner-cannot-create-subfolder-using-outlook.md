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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063136"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Proprietarul nu poate crea sub folder utilizând Outlook

**Există o problemă continuă cu proprietarii de foldere publice, care creează subfoldere utilizând Outlook. Problema va fi remediată în curând.**

Între timp, utilizați una dintre următoarele soluții:

1. Utilizați Outlook mac pentru a crea subfolderul, deoarece problema afectează doar Outlook desktop windows (toate versiunile)
2. Spuneți administratorului să creeze subfolderul utilizând EXO Shell sau EAC
3. Modificați DefaultPublicFolderMailbox/EffectivePublicFolderMailbox a utilizatorului la altă cutie poștală decât cutia poștală de conținut, pentru folderul care provoacă problema  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Așteptați o oră, reporniți clientul Outlook