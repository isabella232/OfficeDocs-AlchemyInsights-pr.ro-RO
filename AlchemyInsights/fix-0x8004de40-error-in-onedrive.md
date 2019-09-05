---
title: Fix 0x8004de40 eroare în OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755860"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Fix 0x8004de40 eroare în OneDrive

Dacă primiți o eroare 0x8004de40 cu OneDrive:

- Reporniți computerul afectat în timp ce sunteți conectat la domeniul Acitve Directory.
- Dacă o repornire nu remediază problema, părăsiţi și realăturați-vă dispozitivul de la Azure AD. 

**Notă**: ar trebui să fiți în rețeaua corporativă în timp ce efectuați acești pași. Nu efectuați acești pași atunci când nu sunteți în măsură să vă conectați la infrastructura corporativă (de exemplu, în timp ce călătoriți). 

- Deschideți un prompt de comandă privilegiat. 
- Pentru a deschide un prompt de comandă privilegiat, faceți clic pe **Start**, faceți clic dreapta pe **Command Prompt**, apoi faceți clic pe **Executare ca administrator**.
- Tip *dsregcmd/plecare* și pres **Enter**.
- Când complet, tastați *dsregcmd/Join* și apăsați **Enter**.
- Când terminați, închideți promptul de comandă.
- Reporniți computerul și conectați-vă la OneDrive.