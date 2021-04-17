---
title: Depanarea problemelor cu OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826211"
---
# <a name="troubleshoot-onedrive-crashes"></a>Depanarea problemelor cu OneDrive

Dacă OneDrive se blochează în mod repetat, încercați acești pași de depanare:

**Asigurați-vă că nu sunt setate chei de registry:**

1. Utilizând Registry Editor, navigați la HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Dacă DisableFileSyncNGSC este prezent și setat la 1, deschideți cheia și modificați valoarea la 0.
3. Lansați manual OneDrive, în start ![Apăsați tasta Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tastați OneDrive în caseta de căutare, apoi faceți clic pe aplicația desktop OneDrive.

**Resetați OneDrive:**

Note:

- Resetarea OneDrive deconectează toate conexiunile de sincronizare existente (inclusiv contul OneDrive personal, dacă este configurat).
- Nu veți pierde fișiere sau date în cazul resetării OneDrive pe computer.

**Pentru a reseta OneDrive:**

1. Deschideți o casetă de dialog Executare, apăsând tasta Windows și R.
2. Tastați %localappdata%\Microsoft\OneDrive\onedrive.exe /reset și apăsați OK. Poate apărea o fereastră de comandă pentru un timp scurt.
3. Lansați manual OneDrive, în start ![Apăsați tasta Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tastați OneDrive în caseta de căutare, apoi faceți clic pe aplicația desktop OneDrive.

Note:

- Dacă ați ales să sincronizați doar unele foldere înainte de a reseta, va trebui să faceți acest lucru din nou după ce se încheie sincronizarea. Citiți [Alegeți ce foldere OneDrive să se sincronizeze cu computerul dvs.](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   pentru mai multe informații.
- Va trebui să faceți acest lucru pentru contul OneDrive personal și pentru OneDrive pentru business.