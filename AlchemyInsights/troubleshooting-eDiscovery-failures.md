---
title: 1490-depanare-eDiscovery-eșecuri
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277824"
---
# <a name="troubleshoot-content-search-errors"></a>Depanarea erorilor de căutare a conținutului

Întâmpinați probleme cu căutarea de conținut sau cu eșecurile atunci când exportați rezultatele căutării?

De exemplu, primiți următoarele la executarea căutărilor?

- CS008 sau CS012 erori

- Erori de Server ocupat/de expirare

- A apărut eroarea de aplicație

Sau atunci când căutați sau exportați rezultate dintr-un număr mare de cutii poștale (peste 100.000 de cutii poștale), primiți erori de export?

Pentru aceste tipuri de erori, încercați din nou căutarea locațiilor de conținut care nu au reușit. Pentru mai multe informații, consultați  [acest articol](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .

Dacă exportați mai mult de 100K cutii poștale, va trebui să utilizați următorul PowerShell pentru a descărca rezultatele de export:  [Exportul rezultatelor din mai mult de 100k cutii poștale](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
