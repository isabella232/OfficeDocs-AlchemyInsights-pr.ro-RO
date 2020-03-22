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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891761"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook nu se poate conecta la foldere publice

Dacă accesul la foldere publice nu funcționează pentru unii utilizatori, încercați următoarele:

Conectați-vă la EXO PowerShell și configurați parametrul DefaultPublicFolderMailbox pe contul de utilizator problemă pentru a se potrivi parametrului pe un cont de utilizator de lucru.

Exemplu:

Ia-Cutie poștală WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<valoare din comanda anterioară>

Așteptați cel puțin o oră pentru ca modificarea să aibă efect.

Dacă problema rămâne, urmați [această procedură](https://aka.ms/pfcte) pentru a depana problemele de acces la folderele publice utilizând Outlook.