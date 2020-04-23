---
title: Remedierea erorii 0x8004de40 în OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716040"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Remedierea erorii 0x8004de40 în OneDrive

Dacă primiți o eroare 0x8004de40 cu OneDrive:

- Reporniți computerul afectat în timp ce conectat la domeniul Director Acitve.
- Dacă o repornire nu remediază problema, unjoin și realăturați-vă dispozitivul de la Azure AD. 

**Notă:** Ar trebui să fie în rețeaua de corporate în timp ce efectuați acești pași. Nu efectuați acești pași atunci când nu vă puteți conecta la infrastructura companiei (de exemplu, în timpul călătoriei). 

- Deschideți un prompt de comandă privilegiat. 
- Pentru a deschide un prompt de comandă privilegiat, faceți clic pe **Start**, faceți clic cu butonul din dreapta pe **Linie de comandă**, apoi faceți clic pe Executare ca **administrator**.
- Tastați *dsregcmd /leave* și apăsați **Enter**.
- Când terminați, tastați *dsregcmd /join* și apăsați **Enter**.
- Când terminați, închideți promptul de comandă.
- Reporniți computerul și conectați-vă la OneDrive.