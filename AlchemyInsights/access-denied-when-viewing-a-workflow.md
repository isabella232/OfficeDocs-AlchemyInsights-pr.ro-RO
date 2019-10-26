---
title: Acces refuzat la vizualizarea unui flux de lucru
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747760"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="fc03d-102">Acces refuzat la vizualizarea unui flux de lucru</span><span class="sxs-lookup"><span data-stu-id="fc03d-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="fc03d-103">SharePoint 2013 fluxuri de lucru care încearcă să trimiteți un e-mail la un grup SharePoint poate eșua cu un mesaj de eroare "Access Denied" Dacă apartenența la grupul SharePoint nu este setată la toată lumea.</span><span class="sxs-lookup"><span data-stu-id="fc03d-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="fc03d-104">**Pentru a rezolva această problemă, urmați acești pași:**</span><span class="sxs-lookup"><span data-stu-id="fc03d-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="fc03d-105">Permiteți tuturor să vadă membrii grupului SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fc03d-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="fc03d-106">Eliminați grupul SharePoint din linia către sau CC a e-mailului.</span><span class="sxs-lookup"><span data-stu-id="fc03d-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="fc03d-107">Adăugați în mod explicit utilizatorii la linia către sau CC dacă vizibilitatea apartenenței nu se poate modifica pentru grupul SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fc03d-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="fc03d-108">Pentru a vedea mai multe detalii, vă rugăm să consultați [http neautorizat la/_vti_bin/client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="fc03d-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  