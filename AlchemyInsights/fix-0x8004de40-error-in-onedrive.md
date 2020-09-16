---
title: Remedierea erorii 0x8004de40 în OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745142"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Remedierea erorii 0x8004de40 în OneDrive

Dacă primiți o eroare 0x8004de40 cu OneDrive:

- Reporniți computerul afectat în timp ce sunteți conectat la domeniul directorului Acitve.
- Dacă repornirea nu rezolvă problema, anulați asocierea și reasocierea dispozitivului din Azure AD. 

**Notă**: trebuie să fiți în rețeaua corporativă în timp ce efectuați acești pași. Nu efectuați acești pași atunci când nu vă puteți conecta la infrastructura firmei (de exemplu, în timpul călătoriei). 

- Deschideți un prompt de comandă privilegiat. 
- Pentru a deschide o linie de comandă privilegiat, faceți clic pe- **Start**, faceți clic dreapta pe **linie de comandă**, apoi faceți clic pe **rulare ca administrator**.
- Tastați *dsregcmd/Leave* și apăsați pe **Enter**.
- Când terminați, tastați *dsregcmd/Join* și apăsați pe **Enter**.
- Când terminați, închideți linia de comandă.
- Reporniți computerul și conectați-vă la OneDrive.