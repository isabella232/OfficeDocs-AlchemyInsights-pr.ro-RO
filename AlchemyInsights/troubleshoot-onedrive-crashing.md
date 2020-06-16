---
title: Depanarea căderilor OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749166"
---
# <a name="troubleshoot-onedrive-crashes"></a>Depanarea căderilor OneDrive

Dacă OneDrive se blochează în mod repetat, încercați acești pași de depanare:

**Asigurați-vă că cheile de registry nu sunt setate:**

1. Utilizând Registry Editor, navigați la HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Dacă DisableFileSyncNGSC este prezent și setat la 1, deschideți cheia și modificați valoarea la 0.
3. Lansați manual OneDrive mergând la Start ![Apăsați tasta Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tastați OneDrive în caseta de căutare, apoi faceți clic pe aplicația desktop OneDrive.

**Reinițializare OneDrive:**

Note:

- Resetarea OneDrive deconectează toate conexiunile de sincronizare existente (inclusiv OneDrive-ul personal, dacă este configurat).
- Nu veți pierde fișiere sau date prin resetarea OneDrive pe computer.

**Pentru a reseta OneDrive:**

1. Deschideți un dialog Executare apăsând tasta Windows și R.
2. Tastați %localappdata%\Microsoft\OneDrive\onedrive.exe /reset și apăsați OK. Este posibil ca o fereastră Comandă să apară pentru scurt timp.
3. Lansați manual OneDrive mergând la Start ![Apăsați tasta Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tastați OneDrive în caseta de căutare, apoi faceți clic pe aplicația desktop OneDrive.

Note:

- Dacă ați ales să sincronizați doar unele foldere înainte de resetare, va trebui să faceți acest lucru din nou după terminarea sincronizării. Citiți [Alegeți ce foldere OneDrive să sincronizați la computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)pentru mai multe   informații.
- Va trebui să finalizați acest lucru pentru OneDrive și OneDrive pentru business personale.