---
title: Depanarea problemelor de import PST
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991378"
---
# <a name="troubleshooting-pst-import-issues"></a>Depanarea problemelor de import PST

- Dacă importați în clientul Outlook însuși, consultați [Remedierea problemelor cu importul unui fișier Outlook .pst](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Dacă utilizați serviciul de import și acesta s-a blocat, rețineți că fiecare fișier PST pe care îl încărcați în locația de stocare Azure nu trebuie să aibă o dimensiune mai mare de 20 GB. Fișierele PST mai mari de 20 GB pot avea un impact asupra performanței procesului de import PST.

- Dacă doriți să verificați starea unei anumite operațiuni de import, puteți utiliza [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Pentru detalii complete despre serviciul de import, consultați [Prezentare generală a importului fișierelor PST ale organizației dvs.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
