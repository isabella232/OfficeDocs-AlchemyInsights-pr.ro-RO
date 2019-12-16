---
title: Depanarea mesajelor de acces refuzat
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050717"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="c1fa3-102">Depanarea mesajelor de acces refuzat</span><span class="sxs-lookup"><span data-stu-id="c1fa3-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="c1fa3-103">Dacă cineva a primit un mesaj "acces refuzat" la un folder partajat în SharePoint, administratorul de colecție de site-ul ar putea fi activat "limitat-acces utilizator permisiunea de blocare modul."</span><span class="sxs-lookup"><span data-stu-id="c1fa3-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="c1fa3-104">Pentru a dezactiva acest lucru:</span><span class="sxs-lookup"><span data-stu-id="c1fa3-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="c1fa3-105">Navigați la site-ul, faceți clic pe pictograma Setări, apoi faceți clic pe **Setări site**.</span><span class="sxs-lookup"><span data-stu-id="c1fa3-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="c1fa3-106">Sub **Administrare colecție de site**-uri, faceți clic pe **Caracteristici colecție site**.</span><span class="sxs-lookup"><span data-stu-id="c1fa3-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="c1fa3-107">Lângă **modul de închidere permisiuni de utilizator limitat**, faceți clic pe **Dezactivare**.</span><span class="sxs-lookup"><span data-stu-id="c1fa3-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="c1fa3-108">Un mesaj de acces refuzat poate apărea, de asemenea, pentru folderele partajate dacă site-ul este un site de publicare.</span><span class="sxs-lookup"><span data-stu-id="c1fa3-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="c1fa3-109">Pentru informații, consultați [accesul refuzat la accesarea unui folder partajat](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="c1fa3-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="c1fa3-110">Dacă cineva a primit un mesaj "Access Denied" atunci când încearcă să vizualizeze solicitările de acces, utilizatorul trebuie să fie adăugat fie ca administrator de colecție de site-uri, fie ca membru al grupului proprietari pentru site.</span><span class="sxs-lookup"><span data-stu-id="c1fa3-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="c1fa3-111">Pentru mai multe informații, consultați [acces refuzat la lista de solicitări de acces](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="c1fa3-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="c1fa3-112">Dacă un utilizator primit un mesaj "Access Denied" după ce au fost eliminate din Active Directory local și apoi adăugat înapoi, consultați [acces refuzat atunci când un cont de utilizator este sincronizat cu Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="c1fa3-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

