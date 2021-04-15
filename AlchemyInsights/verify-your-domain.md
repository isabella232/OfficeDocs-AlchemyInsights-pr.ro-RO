---
title: Verificarea domeniului
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51771003"
---
# <a name="verify-your-domain"></a><span data-ttu-id="94969-102">Verificarea domeniului</span><span class="sxs-lookup"><span data-stu-id="94969-102">Verify your domain</span></span>

 <span data-ttu-id="94969-103">**Probabil că înregistrarea nu s-a actualizat pe internet.**</span><span class="sxs-lookup"><span data-stu-id="94969-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="94969-104">De obicei, durează doar câteva minute pentru ca noi să putem vedea noua înregistrare, dar uneori poate dura câteva ore.</span><span class="sxs-lookup"><span data-stu-id="94969-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="94969-105">Dacă ați așteptat mult timp deja, verificați încă o dublură dacă ați copiat și lipit valoarea exactă în înregistrarea TXT pentru verificarea la gazda DNS.</span><span class="sxs-lookup"><span data-stu-id="94969-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="94969-106">O problemă frecventă este o includere a părții "MS=" a înregistrării.</span><span class="sxs-lookup"><span data-stu-id="94969-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="94969-107">Avem nevoie și de acesta!</span><span class="sxs-lookup"><span data-stu-id="94969-107">We need that too!</span></span>

- <span data-ttu-id="94969-108">Pentru unele gazde DNS, trebuie să urmați un pas suplimentar pentru a salva fișierul de zonă (unde se stochează înregistrarea DNS), astfel încât acesta să se actualizeze pe internet.</span><span class="sxs-lookup"><span data-stu-id="94969-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="94969-109">Asigurați-vă că ați salvat modificările, astfel încât Microsoft să poată vedea și verifica înregistrarea.</span><span class="sxs-lookup"><span data-stu-id="94969-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
