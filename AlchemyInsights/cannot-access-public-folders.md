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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996642"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook se poate conecta la foldere publice

Dacă accesul la folderele publice nu funcționează pentru unii utilizatori, încercați următoarele:

Conectare la EXO PowerShell și configurați parametrul DefaultPublicFolderMailbox în contul de utilizator problemă pentru a se potrivi cu parametrul unui cont de utilizator care lucrează.

Exemplu:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Așteptați cel puțin o oră pentru ca modificarea să aibă efect.

Dacă problema rămâne, urmați această procedură pentru [a depana](https://aka.ms/pfcte) problemele de acces la folderele publice Outlook.
 
**Pentru a controla ce utilizatori pot accesa folderele publice utilizând Outlook:**

1.  Utilizarea Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true sau $false  
      
    $true: Permiteți utilizatorilor să acceseze foldere publice în Outlook  
      
    $false: Împiedicați accesul utilizatorilor la folderele publice din Outlook. Aceasta este valoarea implicită.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Notă** Această procedură poate controla conexiunile doar cu Outlook desktop, Windows clienții. Un utilizator poate continua să acceseze foldere publice utilizând OWA sau Outlook pentru Mac.
 
Pentru mai multe informații, [consultați Anunță suportul pentru Conexiuni controlate la folderele publice din Outlook](https://aka.ms/controlpf).