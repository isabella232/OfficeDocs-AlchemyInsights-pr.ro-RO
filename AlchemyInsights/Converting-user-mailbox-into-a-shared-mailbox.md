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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29485044"
---
<span data-ttu-id="7f002-p101">Puteţi converti numai o cutie poştală de utilizator la o cutie poştală partajată în cazul în care utilizatorul are o licenta de Exchange. După ce căsuţa poştală este convertit, va continua să apară în lista de utilizatori activi, deoarece această listă include cutii poştale partajate. Cu toate acestea, cutia poştală convertit va, de asemenea, apar în lista de cutii poştale partajate.</span><span class="sxs-lookup"><span data-stu-id="7f002-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="7f002-p102">Dacă încercaţi să convertiţi o cutie poştală în consola de administrare Exchange şi conversia eşuează, goliţi memoria cache-ul browser-ul şi cookie-uri şi încercaţi din nou. Dacă încă nu funcţionează, încercaţi să conversia cutia poştală în Exchange Management Shell executând următoarea comandă:</span><span class="sxs-lookup"><span data-stu-id="7f002-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="7f002-107">Mai multe informaţii de conversie cutie poştală este disponibil în [converti o cutie poştală de utilizator la o cutie poştală partajată](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="7f002-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
