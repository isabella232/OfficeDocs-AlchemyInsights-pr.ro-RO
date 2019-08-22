---
title: Convertizor cutie poştală de utilizator într-o cutie poştală partajată?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496447"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Conversia un utilizator de poştă cutie într-o cutie poştală partajată

Puteţi converti numai o cutie poştală de utilizator la o cutie poştală partajată în cazul în care utilizatorul are o licenta de Exchange. După ce căsuţa poştală este convertit, va continua să apară în lista de utilizatori activi, deoarece această listă include cutii poştale partajate. Cu toate acestea, cutia poştală convertit va, de asemenea, apar în lista de cutii poştale partajate. 
  
Dacă încercaţi să convertiţi o cutie poştală în consola de administrare Exchange şi conversia eşuează, goliţi memoria cache-ul browser-ul şi cookie-uri şi încercaţi din nou. Dacă încă nu funcţionează, încercaţi să conversia cutia poştală în Exchange Management Shell executând următoarea comandă:
  
```
Set-Mailbox -Type Shared
```

Mai multe informaţii de conversie cutie poştală este disponibil în [converti o cutie poştală de utilizator la o cutie poştală partajată](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
