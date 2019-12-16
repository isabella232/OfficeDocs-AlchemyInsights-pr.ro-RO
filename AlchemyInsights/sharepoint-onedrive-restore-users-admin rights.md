---
title: Depanarea accesului refuzat mesaje la OneDrive for Business site-uri
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051617"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="e432a-102">Depanarea accesului refuzat mesaje la OneDrive for Business site-uri</span><span class="sxs-lookup"><span data-stu-id="e432a-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="e432a-103">Această problemă apare cel mai frecvent atunci când un utilizator este șters și re-creat cu același nume principal de utilizator (UPN).</span><span class="sxs-lookup"><span data-stu-id="e432a-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="e432a-104">Noul cont este creat utilizând un alt PUID (pașaport Unique ID) valoare.</span><span class="sxs-lookup"><span data-stu-id="e432a-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="e432a-105">Când utilizatorul încearcă să acceseze o colecție de site-uri sau OneDrive lor, utilizatorul are un PUID incorect.</span><span class="sxs-lookup"><span data-stu-id="e432a-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="e432a-106">Un al doilea scenariu implică sincronizare director cu o unitate organizațională Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="e432a-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="e432a-107">Dacă utilizatorii s-au conectat deja la SharePoint și apoi sunt mutate într-un ou diferit și traducerea cu SharePoint, acestea pot experimenta această problemă.</span><span class="sxs-lookup"><span data-stu-id="e432a-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="e432a-108">Pentru a rezolva această problemă ar trebui să restaurați UPN originală cu pașii din articol, [restaurați un utilizator în Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="e432a-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="e432a-109">Dacă nu se poate restaura utilizatorul original ar trebui să eliminați utilizatorul vechi din site-ul OneDrive utilizând acești pași, [Eliminați un utilizator din lista de informații de utilizator]().</span><span class="sxs-lookup"><span data-stu-id="e432a-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="e432a-110">După ce se face acest lucru, aveți posibilitatea să verificați că utilizatorul are drepturi de administrator la site-ul OneDrive urmând pașii pentru a [adăuga admin pentru un utilizator OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="e432a-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="e432a-111">Pentru mai multe informații despre nivelurile de permisiune, consultați articolul, [înțelegerea nivelurilor de permisiune în SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="e432a-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
