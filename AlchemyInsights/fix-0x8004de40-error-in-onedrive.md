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
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133988"
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