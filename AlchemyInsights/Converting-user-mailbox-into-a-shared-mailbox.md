---
title: Convertizor cutie poştală de utilizator într-o cutie poştală partajată?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28307610"
---
Puteţi converti numai o cutie poştală de utilizator la o cutie poştală partajată în cazul în care utilizatorul are o licenta de Exchange. După ce căsuţa poştală este convertit, va continua să apară în lista de utilizatori activi, deoarece această listă include cutii poştale partajate. Cu toate acestea, cutia poştală convertit va, de asemenea, apar în lista de cutii poştale partajate. 
  
Dacă încercaţi să convertiţi o cutie poştală în consola de administrare Exchange şi conversia eşuează, goliţi memoria cache-ul browser-ul şi cookie-uri şi încercaţi din nou. Dacă încă nu funcţionează, încercaţi să conversia cutia poştală în Exchange Management Shell executând următoarea comandă:
  
```
Set-Mailbox -Type Shared
```

Mai multe informaţii de conversie cutie poştală este disponibil în [converti o cutie poştală de utilizator la o cutie poştală partajată](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
