---
title: Permisiuni pentru calendar
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
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046116"
---
# <a name="calendar-permissions"></a>Permisiuni pentru calendar

Utilizatorii își pot modifica propriile Permisiuni de calendar cu Outlook pe web sau cu alți clienți, dar, în calitate de administrator, poate fi necesar să investigați și dvs.  
Cu Exchange PowerShell vă va arăta permisiunea pentru calendarul unui utilizator:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Pentru a vedea mai multe informații, consultați următoarele:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Permisiunile de calendar sunt utilizate în partajarea calendarelor. Pentru a vedea mai multe informații despre partajarea unui calendar Outlook, consultați aceste articole:

- [Partajarea unui calendar Outlook cu alte persoane](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Partajarea calendarului în Outlook pe web pentru firme](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Pentru a depana Permisiunea de [calendar, puteți Asistent pentru recuperare și asistență](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) de calendar.