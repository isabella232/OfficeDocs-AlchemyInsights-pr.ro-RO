---
title: Depanarea OneDrive de erori
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
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921019"
---
# <a name="troubleshoot-onedrive-crashes"></a>Depanarea OneDrive de erori

Dacă OneDrive se blochează în mod repetat, încercați acești pași de depanare:

**Asigurați-vă că nu sunt setate chei de registry:**

1. Utilizând Registry Editor, navigați la HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Dacă DisableFileSyncNGSC este prezent și setat la 1, deschideți cheia și modificați valoarea la 0.
3. Lansați manual OneDrive, în meniul Start ![Apăsați tasta Windows cheie](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tastați OneDrive în caseta de căutare, apoi faceți clic pe OneDrive desktop.

**Resetați OneDrive:**

Note:

- Resetarea OneDrive deconectează toate conexiunile de sincronizare existente (inclusiv contul personal OneDrive dacă sunt configurate).
- Nu veți pierde fișiere sau date în funcție de resetarea OneDrive computer.

**Pentru a reseta OneDrive:**

1. Deschideți o casetă de dialog Executare, apăsând tasta Windows și R.
2. Tastați %localappdata%\Microsoft\OneDrive\onedrive.exe /reset și apăsați OK. Poate apărea o fereastră de comandă pentru un timp scurt.
3. Lansați manual OneDrive, în meniul Start ![Apăsați tasta Windows cheie](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tastați OneDrive în caseta de căutare, apoi faceți clic pe OneDrive desktop.

Note:

- Dacă ați ales să sincronizați doar unele foldere înainte de a reseta, va trebui să faceți acest lucru din nou după ce se încheie sincronizarea. Citiți [Alegeți ce OneDrive să se sincronizeze cu computerul dvs.](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   pentru mai multe informații.
- Va trebui să faceți acest lucru pentru contul dvs. OneDrive a OneDrive pentru business.