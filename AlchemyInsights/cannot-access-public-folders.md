---
title: Imposibil de accesat folderele publice
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
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819524"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook nu se poate conecta la folderele publice

Dacă accesul la folderele publice nu funcționează pentru unii utilizatori, încercați următoarele:

Conectați-vă la EXO PowerShell și configurați parametrul DefaultPublicFolderMailbox pe contul de utilizator problemă pentru a se potrivi cu parametrul unui cont de utilizator care lucrează.

Exemplu:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Așteptați cel puțin o oră pentru ca modificarea să aibă efect.

Dacă problema rămâne, urmați această procedură pentru [a depana](https://aka.ms/pfcte) problemele de acces la folderele publice utilizând Outlook.
 
**Pentru a controla ce utilizatori pot accesa folderele publice utilizând Outlook:**

1.  Utilizarea Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true sau $false  
      
    $true: Permiteți utilizatorilor să acceseze foldere publice în Outlook  
      
    $false: Împiedicarea accesului utilizatorilor la folderele publice în Outlook. Aceasta este valoarea implicită.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Notă** Această procedură poate controla conexiunile doar cu clienții Outlook pentru desktop pentru Windows. Un utilizator poate continua să acceseze folderele publice utilizând OWA sau Outlook pentru Mac.
 
Pentru mai multe informații, [consultați Anunțarea suportului pentru Conexiuni controlate la folderele publice din Outlook.](https://aka.ms/controlpf)