---
title: Probleme de permisiuni în timpul migrării
ms.author: pebaum
author: Techwriter40
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 33e605ff3019f52bbd0be876d485ff389b260a44
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752620"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="5c1c0-102">Sincronizarea profilului de utilizator și a fotografiilor</span><span class="sxs-lookup"><span data-stu-id="5c1c0-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="5c1c0-103">**Profil Sincronizarea fotografiilor** -utilizatorii pot observa că fotografia lor de profil nu este sincronizarea la SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="5c1c0-104">Sau, ele pot fi încercat să actualizeze fotografia lor de profil și fotografia încă apare ca fotografie vechi.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="5c1c0-105">Pentru a vă asigura că fotografia de profil Arată conform așteptărilor, utilizatorul va trebui să inițieze o sincronizare foto.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="5c1c0-106">Pentru mai multe informații despre procesul de sincronizare a fotografiilor, consultați [informații despre sincronizarea imaginii de profil în Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="5c1c0-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="5c1c0-107">**Sincronizarea profilului** -timpul necesar pentru finalizarea sincronizării profilului depinde de numărul de modificări (de lucru) pe care trebuie să le proceseze lucrarea de import AD.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="5c1c0-108">Dacă există multe modificări, activitatea de cronometrare are o mulțime de lucru de făcut și va dura mai mult pentru ca modificările să se reflecte în aplicația profil utilizator.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="5c1c0-109">Dacă activitatea de cronometrare are un volum mic de lucru de făcut, modificările vor fi reflectate în aplicația profil utilizator mult mai rapid.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="5c1c0-110">Pentru mai multe informații despre procesul de sincronizare profil, consultați [informații despre sincronizarea profilului de utilizator în SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="5c1c0-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="5c1c0-111">**Actualizare profil în Office Delve** -Delve utilizatorii pot gestiona lor Office 365 profil.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="5c1c0-112">Pentru mai multe informații, consultați [vizualizarea și actualizarea profilului în Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="5c1c0-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

