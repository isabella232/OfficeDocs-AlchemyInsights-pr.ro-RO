---
title: Imposibil de accesat folderele publice
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
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959506"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook nu se poate conecta la foldere publice

Dacă accesul public folder nu funcționează pentru puțini utilizatori, încercați următoarele:

Conectați-vă la EXO PowerShell și configurați DefaultPublicFolderMailbox pe contul de utilizator problema pentru a se potrivi cu unul pe un cont de utilizator de lucru.

Exemplu:

Get-cutie poștală WorkingUser | ft DefaultPublicFolderMailbox, Efectivepublicfoldermailbox

Set-Mailbox Problemusutilizator-DefaultPublicFolderMailbox \<valoare de la comanda anterioară>

Așteptați cel puțin o oră pentru ca modificarea să aibă efect.