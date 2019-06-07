---
title: 1336 RecoverableItems dosarul este complet
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: cfcc69c1b3a59c73037d9a493af4ece86b7b7208
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762092"
---
# <a name="the-recoverable-items-folder-is-full"></a>Folderul Elemente recuperabile este plin

Pentru poştale Exchange Online în Office 365, limita de stocare implicită pentru folderul Elemente recuperabile este 30 GB. Limita de stocare pentru folderul Elemente recuperabile este crescut automat la 100 GB, în cazul în care cutia poştală este plasat litigii Hold, ţineţi eDiscovery, sau este asociată o politică de retenție Office 365.

Când folderul Elemente recuperabile atinge limita de stocare, funcţionalitatea de cutie poştală este afectată în următoarele moduri:

- Utilizatorul nu poate şterge elemente din cutia poştală.

- Asistentul pentru foldere gestionate nu se poate şterge elemente bazate pe etichetă de conservare sau setările de foldere gestionate.

- Pentru cutiile poştale care au singur element recuperare permis sau sunt puse pe "hold", procesul de protecţie copia pe scrie filme nu poate menține versiuni de articole editate de catre utilizator.

- Pentru cutiile poştale care au cutii poştale activate de logare de audit, nici o cutie poştală de audit intrări jurnal pot fi salvate în subfolderul de audit din folderul Elemente recuperabile.

Pentru cutiile poştale care nu sunt pe "hold", puteţi utiliza administratori `Search-Mailbox -SearchDumpsterOnly -DeleteContent` comanda în Exchange Online PowerShell să ştergeţi elementele din folderul Elemente recuperabile. Pentru informații suplimentare, consultați următoarele articole: 

- [Căuta şi a şterge mesaje](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Cutia poştală de căutare](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Pentru cutiile poştale care sunt pe "hold", administratorii trebuie să eliminaţi Cala înainte ei a putea elementele şterse din folderul Elemente recuperabile. Pentru informaţii suplimentare, consultaţi [ştergeţi elementele din Elemente recuperabile folderul de cutii poştale din cadrul norului pe hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Pentru a preveni folderul Elemente recuperabile de a deveni complet, administratorii pot creşte limita de stocare de Elemente recuperabile pliant pentru cutiile poştale pe hold şi a înfiinţat o cutie poştală conservare care mută elementele din folderul Elemente recuperabile al utilizatorului Arhiva cutie poştală. Consultaţi [creşte Elemente recuperabile cotelor pentru cutii poştale pe hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
