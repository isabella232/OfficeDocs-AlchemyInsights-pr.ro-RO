---
title: Nu puteți accesa folderele publice
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
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812559"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook nu se poate conecta la folderele publice

Dacă accesul la foldere publice nu funcționează pentru unii utilizatori, încercați următoarele:

Conectați-vă la EXO PowerShell și configurați parametrul DefaultPublicFolderMailbox pe contul de utilizator al problemei pentru a se potrivi cu parametrul pentru un cont de utilizator care funcționează.

Exemplu

WorkingUser de primire a cutiei poștale | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-cutia poștală ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Așteptați cel puțin o oră pentru ca modificarea să aibă efect.

Dacă problema rămâne, vă rugăm să urmați [această procedură](https://aka.ms/pfcte) pentru a depana problemele de acces la foldere publice utilizând Outlook.
 
**Pentru a controla ce utilizatori pot accesa folderele publice utilizând Outlook**:

1.  Utilizați Set-CASMailbox <mailboxname> -PublicFolderClientAccess $True sau $false  
      
    $true: Permiteți utilizatorilor să acceseze folderele publice în Outlook  
      
    $false: împiedicați accesul utilizatorilor la foldere publice în Outlook. Aceasta este valoarea implicită.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Notă** Această procedură poate controla conexiunile doar cu clienții Outlook desktop pentru Windows. Un utilizator poate continua să acceseze foldere publice folosind OWA sau Outlook pentru Mac.
 
Pentru mai multe informații, consultați [anunțarea acceptării conexiunilor controlate la foldere publice în Outlook](https://aka.ms/controlpf).