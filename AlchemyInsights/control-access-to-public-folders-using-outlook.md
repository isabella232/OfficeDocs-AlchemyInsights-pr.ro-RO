---
title: Controlul accesului la folderele publice utilizând Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032570"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Controlul accesului la folderele publice utilizând Outlook

Pentru a controla ce utilizatori pot accesa folderele publice utilizând Outlook:

1. Utilizare `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Permiteți utilizatorilor să acceseze foldere publice în Outlook  
$false: Împiedicați accesul utilizatorilor la folderele publice din Outlook. Aceasta este valoarea implicită.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Notă: Această procedură poate controla doar conexiunile Outlook desktop pentru Windows clienți. Utilizatorii pot continua să acceseze foldere publice utilizând OWA sau Outlook pentru Mac.

Pentru mai multe informații, [consultați Conexiuni controlate la folderele publice din Outlook](https://aka.ms/controlpf) mai multe informații.
