---
title: Depanarea mesajelor refuzate la acces
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759812"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="1fd7c-102">Depanarea mesajelor refuzate la acces</span><span class="sxs-lookup"><span data-stu-id="1fd7c-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="1fd7c-103">Dacă cineva a primit un mesaj "Acces refuzat" într-un folder partajat din SharePoint, este posibil ca administratorul colecției de site-uri să fi activat "Modul de blocare a permisiunii de utilizator cu acces limitat".</span><span class="sxs-lookup"><span data-stu-id="1fd7c-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="1fd7c-104">Pentru a dezactiva această dezactivare:</span><span class="sxs-lookup"><span data-stu-id="1fd7c-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="1fd7c-105">Navigați la site, faceți clic pe pictograma Setări, apoi faceți clic pe **Setări site**.</span><span class="sxs-lookup"><span data-stu-id="1fd7c-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="1fd7c-106">Sub **Administrare colecție de site-uri**, faceți clic pe Caracteristici colecție de **site-uri**.</span><span class="sxs-lookup"><span data-stu-id="1fd7c-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="1fd7c-107">Lângă **Mod de blocare a permisiunii de utilizator cu acces limitat,** faceți clic pe **Dezactivare**.</span><span class="sxs-lookup"><span data-stu-id="1fd7c-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="1fd7c-108">Un mesaj de acces refuzat poate apărea, de asemenea, pentru folderele partajate dacă site-ul este un site de publicare.</span><span class="sxs-lookup"><span data-stu-id="1fd7c-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="1fd7c-109">Pentru informații, consultați [Acces refuzat la accesarea unui folder partajat](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="1fd7c-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="1fd7c-110">Dacă o persoană a primit un mesaj "Acces refuzat" atunci când încearcă să vizualizeze solicitările de acces, utilizatorul trebuie să fie adăugat fie ca administrator de colecție de site-uri, fie ca membru al grupului Proprietari pentru site.</span><span class="sxs-lookup"><span data-stu-id="1fd7c-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="1fd7c-111">Pentru mai multe informații, consultați [Lista acces refuzat la solicitări de acces](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="1fd7c-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="1fd7c-112">Dacă un utilizator a primit un mesaj "Access Denied" după ce au fost eliminate din Active Directory local și apoi adăugat înapoi, consultați [Access Denied atunci când un cont de utilizator este sincronizat cu Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="1fd7c-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

