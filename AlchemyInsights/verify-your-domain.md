---
title: Verificați-vă domeniul
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710455"
---
# <a name="verify-your-domain"></a><span data-ttu-id="fa26a-102">Verificați-vă domeniul</span><span class="sxs-lookup"><span data-stu-id="fa26a-102">Verify your domain</span></span>

 <span data-ttu-id="fa26a-103">**Înregistrarea, probabil, nu sa actualizat pe Internet.**</span><span class="sxs-lookup"><span data-stu-id="fa26a-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="fa26a-104">De obicei durează doar câteva minute pentru ca noi să putem vedea noul record, dar ocazional poate dura până la câteva ore.</span><span class="sxs-lookup"><span data-stu-id="fa26a-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="fa26a-105">Dacă ați așteptat deja atât de mult, verificați de două ori dacă ați copiat și ați lipit valoarea exactă în înregistrarea de verificare TXT de la gazda DNS.</span><span class="sxs-lookup"><span data-stu-id="fa26a-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="fa26a-106">O problemă comună nu include partea "MS=" a înregistrării.</span><span class="sxs-lookup"><span data-stu-id="fa26a-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="fa26a-107">Și noi avem nevoie de asta!</span><span class="sxs-lookup"><span data-stu-id="fa26a-107">We need that too!</span></span>

- <span data-ttu-id="fa26a-108">La unele gazde DNS, trebuie să faceți un pas suplimentar pentru a salva fișierul de zonă (unde este stocată înregistrarea DNS), astfel încât să se actualizeze pe Internet.</span><span class="sxs-lookup"><span data-stu-id="fa26a-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="fa26a-109">Asigurați-vă că ați salvat modificările, astfel încât Microsoft să poată vedea și verifica înregistrarea.</span><span class="sxs-lookup"><span data-stu-id="fa26a-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
