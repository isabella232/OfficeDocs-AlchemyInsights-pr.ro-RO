---
title: Permisiuni calendar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862170"
---
# <a name="calendar-permissions"></a>Permisiuni calendar

Utilizatorii își pot modifica propriile permisiuni de calendar cu Outlook pe Web sau alți clienți, dar, în calitate de administrator, poate fi necesar să investigați și dvs.  
Cu cmdlet Exchange PowerShell vă va arăta permisiunea în calendarul unui utilizator:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Pentru a vedea mai multe informații, consultați următoarele:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Setare-Cutie PoștalăFolderPermisie](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Program de completare-cutie poștalăPermisie](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Permisiunile de calendar sunt utilizate în partajarea calendarelor, pentru a vedea mai multe informații despre partajarea unui calendar Outlook, consultați aceste articole:

- [Partajarea unui calendar Outlook cu alte persoane](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Partajarea calendarului în Outlook pe web pentru firme](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Pentru a depana Permisiunea calendarului, puteți utiliza instrumentul [Asistent asistență și recuperare.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)