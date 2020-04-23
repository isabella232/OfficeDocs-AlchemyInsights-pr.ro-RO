---
title: Probleme de permisiuni în timpul migrării
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 077b7cf29ef6a40ef7f2aebef15e39a0f5df0fc3
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758982"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="f3151-102">Sincronizare profil utilizator și fotografie</span><span class="sxs-lookup"><span data-stu-id="f3151-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="f3151-103">**Sincronizare a fotografiilor de profil** - utilizatorii pot observa că fotografia lor de profil nu se sincronizează cu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f3151-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="f3151-104">Sau, ei pot fi încercat să actualizeze fotografia lor de profil și fotografia încă apare ca fotografie vechi.</span><span class="sxs-lookup"><span data-stu-id="f3151-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="f3151-105">Pentru a se asigura că fotografia de profil se afișează conform așteptărilor, utilizatorul va trebui să inițieze o sincronizare a fotografiilor.</span><span class="sxs-lookup"><span data-stu-id="f3151-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="f3151-106">Pentru mai multe informații despre procesul de sincronizare a fotografiilor, consultați [Informații despre sincronizarea imaginilor de profil în Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="f3151-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="f3151-107">**Sincronizare profil** - Timpul necesar pentru finalizarea unei sincronizări de profil depinde de numărul de modificări (lucru) pe care trebuie să le proceseze lucrarea de import AD.</span><span class="sxs-lookup"><span data-stu-id="f3151-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="f3151-108">Dacă există multe modificări, activitatea de cronometrare are mult de lucru și va dura mai mult pentru ca modificările să se reflecte în aplicația Profil utilizator.</span><span class="sxs-lookup"><span data-stu-id="f3151-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="f3151-109">Dacă activitatea de cronometrare are un volum mic de lucru de făcut, modificările se vor reflecta în aplicația profil utilizator mult mai repede.</span><span class="sxs-lookup"><span data-stu-id="f3151-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="f3151-110">Pentru mai multe informații despre procesul de sincronizare profil, consultați [Informații despre sincronizarea profilului de utilizator în SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="f3151-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="f3151-111">**Actualizare profil în Office Delve** - Utilizatorii Delve pot gestiona profilul Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f3151-111">**Update Profile in Office Delve** - Delve users can manage their Microsoft 365 Profile.</span></span> <span data-ttu-id="f3151-112">Pentru mai multe informații, consultați [Vizualizarea și actualizarea profilului în Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="f3151-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

