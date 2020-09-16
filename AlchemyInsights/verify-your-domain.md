---
title: Verificarea domeniului
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734318"
---
# <a name="verify-your-domain"></a><span data-ttu-id="a3279-102">Verificarea domeniului</span><span class="sxs-lookup"><span data-stu-id="a3279-102">Verify your domain</span></span>

 <span data-ttu-id="a3279-103">**Probabil că înregistrarea nu a fost actualizată pe Internet.**</span><span class="sxs-lookup"><span data-stu-id="a3279-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="a3279-104">De obicei, durează doar câteva minute pentru ca noi să putem vedea noua înregistrare, dar uneori poate dura până la câteva ore.</span><span class="sxs-lookup"><span data-stu-id="a3279-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="a3279-105">Dacă ați așteptat deja atât de mult, verificați de două ori că ați copiat și ați inserat valoarea exactă în înregistrarea de verificare TXT de la gazda DNS.</span><span class="sxs-lookup"><span data-stu-id="a3279-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="a3279-106">O problemă obișnuită nu include partea "MS =" a înregistrării.</span><span class="sxs-lookup"><span data-stu-id="a3279-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="a3279-107">Ne trebuie și asta!</span><span class="sxs-lookup"><span data-stu-id="a3279-107">We need that too!</span></span>

- <span data-ttu-id="a3279-108">La unele gazde DNS, trebuie să faceți un pas suplimentar pentru a salva fișierul de zonă (unde este stocat înregistrarea DNS), astfel încât să se actualizeze pe Internet.</span><span class="sxs-lookup"><span data-stu-id="a3279-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="a3279-109">Asigurați-vă că ați salvat modificările, astfel încât Microsoft să poată vedea și verifica înregistrarea.</span><span class="sxs-lookup"><span data-stu-id="a3279-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
