---
title: Depanarea mesajelor interzise în Access
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704906"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="4863e-102">Depanarea mesajelor interzise în Access</span><span class="sxs-lookup"><span data-stu-id="4863e-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="4863e-103">Dacă cineva a primit un mesaj "acces refuzat" la un folder partajat din SharePoint, este posibil ca administratorul colecției de site-uri să fi activat "modul de blocare a permisiunii pentru utilizatorul Access limitat".</span><span class="sxs-lookup"><span data-stu-id="4863e-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="4863e-104">Pentru a dezactiva această problemă:</span><span class="sxs-lookup"><span data-stu-id="4863e-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="4863e-105">Navigați la site, faceți clic pe pictograma Setări, apoi faceți clic pe **Setări site**.</span><span class="sxs-lookup"><span data-stu-id="4863e-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="4863e-106">Sub **Administrare colecție de site-uri**, faceți clic pe **Caracteristici colecție de site-uri**.</span><span class="sxs-lookup"><span data-stu-id="4863e-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="4863e-107">Lângă **modul blocare permisiune utilizator cu acces limitat**, faceți clic pe **Dezactivare**.</span><span class="sxs-lookup"><span data-stu-id="4863e-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="4863e-108">De asemenea, se poate produce un mesaj de acces refuzat pentru folderele partajate, dacă site-ul este un site de publicare.</span><span class="sxs-lookup"><span data-stu-id="4863e-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="4863e-109">Pentru informații, consultați [Access Denied atunci când accesați un folder partajat](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span><span class="sxs-lookup"><span data-stu-id="4863e-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="4863e-110">Dacă o persoană a primit un mesaj "acces refuzat" atunci când încercați să vizualizați solicitările de acces, utilizatorul trebuie să fie adăugat ca administrator al colecției de site-uri sau ca membru al grupului de proprietari pentru site.</span><span class="sxs-lookup"><span data-stu-id="4863e-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="4863e-111">Pentru mai multe informații, consultați [lista de solicitări Access Denied în Access](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="4863e-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="4863e-112">Dacă un utilizator a primit un mesaj "acces refuzat" după ce a fost eliminat din Active Directory local, apoi s-a adăugat înapoi, consultați [Access Denied când un cont de utilizator este sincronizat la Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="4863e-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

