---
title: Depanarea căderilor OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665010"
---
# <a name="troubleshoot-onedrive-crashes"></a>Depanarea căderilor OneDrive

Dacă OneDrive se defectează în mod repetat, încercați acești pași de depanare:

**Asigurați-vă că nu sunt setate cheile de registry:**

1. Utilizarea Registry Editor, navigați la HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Dacă DisableFileSyncNGSC este prezent și setat la 1, deschideți cheia și modificați valoarea la 0.
3. Lansați manual OneDrive accesând Start ![Apăsați tasta Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tastați OneDrive în caseta de căutare, apoi faceți clic pe aplicația desktop OneDrive.

**Reinițializați OneDrive:**

Note

- Resetarea OneDrive deconectează toate conexiunile de sincronizare existente (inclusiv OneDrive personal, dacă este configurat).
- Nu veți pierde fișiere sau date prin reinițializarea OneDrive pe computer.

**Pentru a reseta OneDrive:**

1. Deschideți o casetă de dialog rulare apăsând tasta Windows și R.
2. Tastați% localappdata% \Microsoft\OneDrive\onedrive.exe/Reset și apăsați pe OK. O fereastră de comandă poate apărea pe scurt.
3. Lansați manual OneDrive accesând Start ![Apăsați tasta Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tastați OneDrive în caseta de căutare, apoi faceți clic pe aplicația desktop OneDrive.

Note

- Dacă ați ales să sincronizați doar unele foldere înainte de resetare, va trebui să faceți acest lucru din nou după ce sincronizarea s-a finalizat. Citiți [Alegeți ce foldere OneDrive să se sincronizeze cu computerul](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   pentru mai multe informații.
- Va trebui să terminați acest lucru pentru OneDrive personal și OneDrive pentru Business.