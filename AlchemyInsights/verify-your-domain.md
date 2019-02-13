---
title: Verifica domeniu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 7332650d1763e2bbd13be48f406fb04b8849a6c1
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29911244"
---
# <a name="verify-your-domain"></a><span data-ttu-id="52eb6-102">Verifica domeniu</span><span class="sxs-lookup"><span data-stu-id="52eb6-102">Verify your domain</span></span>

 <span data-ttu-id="52eb6-103">**Înregistrare, probabil, nu a actualizat pe Internet.**</span><span class="sxs-lookup"><span data-stu-id="52eb6-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="52eb6-104">De obicei durează doar câteva minute pentru a ne putea vedea noua înregistrare, dar ocazional poate dura atâta timp cât câteva ore.</span><span class="sxs-lookup"><span data-stu-id="52eb6-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="52eb6-p101">Dacă aţi aşteptat că mult timp deja, verificaţi că le-am copiat şi inserat valoarea exactă în înregistrări de verificare TXT la gazda dumneavoastra de DNS. Nu este o problemă comună, inclusiv "MS =" o parte din înregistrarea. Am nevoie de asta!</span><span class="sxs-lookup"><span data-stu-id="52eb6-p101">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host. One common issue is not including the "MS=" part of the record. We need that too!</span></span>
    
- <span data-ttu-id="52eb6-p102">La unele servere de DNS, trebuie să ia un pas suplimentar pentru a salva fişierul de zonă (în cazul în care este stocat înregistrarea DNS) astfel încât acesta va actualiza pe Internet. Asiguraţi-vă că ați salvat modificările astfel încât Office 365 pot vedea şi să verifice înregistrarea.</span><span class="sxs-lookup"><span data-stu-id="52eb6-p102">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet. Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

