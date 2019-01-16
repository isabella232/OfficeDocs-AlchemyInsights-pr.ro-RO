---
title: Acces interzis atunci când vizualizaţi un flux de lucru
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28306795"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="a5c63-102">Acces interzis atunci când vizualizaţi un flux de lucru</span><span class="sxs-lookup"><span data-stu-id="a5c63-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="a5c63-103">SharePoint 2013 fluxurile de lucru care încerca să trimiteţi un email la un grup SharePoint poate eşua cu un mesaj de eroare "Access Denied" în cazul în care calitatea de membru al grupului de SharePoint nu este setată la toată lumea.</span><span class="sxs-lookup"><span data-stu-id="a5c63-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="a5c63-104">**Pentru a rezolva această problemă, efectuaţi aceşti paşi:**</span><span class="sxs-lookup"><span data-stu-id="a5c63-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="a5c63-105">Permite toată lumea să vadă membrii grup SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5c63-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="a5c63-106">Elimina grup SharePoint de către sau CC linie de e-mail.</span><span class="sxs-lookup"><span data-stu-id="a5c63-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="a5c63-107">Adăugaţi în mod explicit utilizatorilor către sau CC linie în cazul în care vizibilitatea aderarea nu poate fi schimbat pentru grup SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5c63-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="a5c63-108">Pentru a vizualiza mai multe detalii vă rugăm să consultaţi [HTTP neautorizat la /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="a5c63-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

