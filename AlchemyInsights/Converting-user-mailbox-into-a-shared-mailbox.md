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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374335"
---
<span data-ttu-id="5e922-102">Puteţi converti numai o cutie poştală de utilizator la o cutie poştală partajată în cazul în care utilizatorul are o licenta de Exchange.</span><span class="sxs-lookup"><span data-stu-id="5e922-102">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="5e922-103">După ce căsuţa poştală este convertit, va continua să apară în lista de utilizatori activi, deoarece această listă include cutii poştale partajate.</span><span class="sxs-lookup"><span data-stu-id="5e922-103">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="5e922-104">Cu toate acestea, cutia poştală convertit va, de asemenea, apar în lista de cutii poştale partajate.</span><span class="sxs-lookup"><span data-stu-id="5e922-104">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="5e922-105">Dacă încercaţi să convertiţi o cutie poştală în consola de administrare Exchange şi conversia eşuează, goliţi memoria cache-ul browser-ul şi cookie-uri şi încercaţi din nou.</span><span class="sxs-lookup"><span data-stu-id="5e922-105">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="5e922-106">Dacă încă nu funcţionează, încercaţi să conversia cutia poştală în Exchange Management Shell executând următoarea comandă:</span><span class="sxs-lookup"><span data-stu-id="5e922-106">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="5e922-107">Mai multe informaţii de conversie cutie poştală este disponibil în [converti o cutie poştală de utilizator la o cutie poştală partajată](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="5e922-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
