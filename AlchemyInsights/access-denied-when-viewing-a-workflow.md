---
title: Access Denied când Vizualizați un flux de lucru
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688814"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="320da-102">Access Denied când Vizualizați un flux de lucru</span><span class="sxs-lookup"><span data-stu-id="320da-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="320da-103">Fluxurile de lucru SharePoint 2013 care încearcă să trimită un mesaj de e-mail la un grup SharePoint pot eșua cu un mesaj de eroare "Access Denied" Dacă apartenența la grupul SharePoint nu este setată pentru toată lumea.</span><span class="sxs-lookup"><span data-stu-id="320da-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="320da-104">**Pentru a rezolva această problemă, urmați acești pași:**</span><span class="sxs-lookup"><span data-stu-id="320da-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="320da-105">Permiteți tuturor să vadă membrii grupului SharePoint.</span><span class="sxs-lookup"><span data-stu-id="320da-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="320da-106">Eliminați grupul SharePoint din linia către sau CC a e-mailului.</span><span class="sxs-lookup"><span data-stu-id="320da-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="320da-107">Adăugați în mod explicit utilizatorii la linia către sau CC dacă vizibilitatea apartenenței nu poate fi modificată pentru grupul SharePoint.</span><span class="sxs-lookup"><span data-stu-id="320da-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="320da-108">Pentru a vedea mai multe detalii, consultați [http neautorizat pentru/_vti_bin/client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="320da-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  