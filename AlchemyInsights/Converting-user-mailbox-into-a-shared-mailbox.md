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
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906744"
---
Puteţi converti numai o cutie poştală de utilizator la o cutie poştală partajată în cazul în care utilizatorul are o licenta de Exchange. După ce căsuţa poştală este convertit, va continua să apară în lista de utilizatori activi, deoarece această listă include cutii poştale partajate. Cu toate acestea, cutia poştală convertit va, de asemenea, apar în lista de cutii poştale partajate. 
  
Dacă încercaţi să convertiţi o cutie poştală în consola de administrare Exchange şi conversia eşuează, goliţi memoria cache-ul browser-ul şi cookie-uri şi încercaţi din nou. Dacă încă nu funcţionează, încercaţi să conversia cutia poştală în Exchange Management Shell executând următoarea comandă:
  
```
Set-Mailbox -Type Shared
```

Mai multe informaţii de conversie cutie poştală este disponibil în [converti o cutie poştală de utilizator la o cutie poştală partajată](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
