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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816752"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Controlul accesului la folderele publice utilizând Outlook

Pentru a controla ce utilizatori pot accesa folderele publice utilizând Outlook:

1. Utilizare `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Permiteți utilizatorilor să acceseze foldere publice în Outlook  
$false: Împiedicarea accesului utilizatorilor la folderele publice în Outlook. Aceasta este valoarea implicită.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Notă: Această procedură poate controla doar conexiunile cu clienții Outlook pentru desktop pentru Windows. Utilizatorii pot continua să acceseze foldere publice utilizând OWA sau Outlook pentru Mac.

Pentru mai multe informații, [consultați Conexiuni controlate la folderele publice din Outlook pentru](https://aka.ms/controlpf) mai multe informații.
