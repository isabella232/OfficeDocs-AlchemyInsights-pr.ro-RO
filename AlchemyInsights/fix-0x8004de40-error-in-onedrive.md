---
title: Fix 0x8004de40 eroare în OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525071"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Fix 0x8004de40 eroare în OneDrive

Dacă primiţi o eroare de 0x8004de40 cu OneDrive:

- Reporniţi computerul afectat în timp ce conectat la domeniu Acitve Director.
- În cazul în care o repornire nu se rezolvă problema, părăsiţi şi va reintra în aparatul de Azur AD. 

**Notă**: ar trebui să fie pe reţeaua corporativă în timp ce efectuaţi aceşti paşi. Nu efectuaţi aceşti paşi, atunci când nu sunteţi capabil să se conecteze la infrastructurii corporative (de exemplu, în timp ce călătoresc). 

- Deschidere un ascensor virgulă prompt. 
- Pentru a deschide un prompt de comandă, faceţi clic pe - **Start**, faceţi clic dreapta pe **Prompt comandă**şi apoi faceţi clic pe **Executare ca administrator**.
- *Dsregcmd /leave* de tip şi apăsaţi **Enter**.
- Atunci când completă, tastaţi *dsregcmd/Join* şi apăsaţi **Enter**.
- Când complet, închide promptul de comandă.
- Reporniţi computerul, şi intraţi în OneDrive.