---
title: Acces refuzat la vizualizarea unui flux de lucru
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687342"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="06a50-102">Acces refuzat la vizualizarea unui flux de lucru</span><span class="sxs-lookup"><span data-stu-id="06a50-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="06a50-103">Fluxuri de lucru SharePoint 2013 care încearcă să trimită un e-mail la un grup SharePoint poate să nu reușească cu un mesaj de eroare "Access Denied" dacă apartenența la grupul SharePoint nu este setată la toată lumea.</span><span class="sxs-lookup"><span data-stu-id="06a50-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="06a50-104">**Pentru a rezolva această problemă, efectuați acești pași:**</span><span class="sxs-lookup"><span data-stu-id="06a50-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="06a50-105">Permiteți tuturor să vadă membrii grupului SharePoint.</span><span class="sxs-lookup"><span data-stu-id="06a50-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="06a50-106">Eliminați grupul SharePoint din linia Către sau CC a e-mailului.</span><span class="sxs-lookup"><span data-stu-id="06a50-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="06a50-107">Adăugați în mod explicit utilizatorii la linia Către sau CC dacă vizibilitatea apartenență nu poate fi modificată pentru grupul SharePoint.</span><span class="sxs-lookup"><span data-stu-id="06a50-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="06a50-108">Pentru a vizualiza mai multe detalii, vă rugăm să consultați [HTTP Neautorizat la /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="06a50-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  