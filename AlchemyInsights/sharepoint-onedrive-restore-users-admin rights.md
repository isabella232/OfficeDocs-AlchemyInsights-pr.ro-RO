---
title: Depanarea accesului refuzat mesaje la OneDrive pentru site-uri business
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692813"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="a8995-102">Depanarea accesului refuzat mesaje la OneDrive pentru site-uri business</span><span class="sxs-lookup"><span data-stu-id="a8995-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="a8995-103">Această problemă apare cel mai frecvent atunci când un utilizator este șters și recreat cu același nume principal de utilizator (UPN).</span><span class="sxs-lookup"><span data-stu-id="a8995-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="a8995-104">Noul cont este creat utilizând o valoare PUID (Passport Unique ID) diferită.</span><span class="sxs-lookup"><span data-stu-id="a8995-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="a8995-105">Când utilizatorul încearcă să acceseze o colecție de site-ul sau OneDrive lor, utilizatorul are un PUID incorecte.</span><span class="sxs-lookup"><span data-stu-id="a8995-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="a8995-106">Un al doilea scenariu implică sincronizarea directorului cu o unitate organizațională Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="a8995-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="a8995-107">Dacă utilizatorii s-au conectat deja la SharePoint, și apoi sunt mutate într-un alt OU și resynced cu SharePoint, acestea pot apărea această problemă.</span><span class="sxs-lookup"><span data-stu-id="a8995-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="a8995-108">Pentru a rezolva această problemă ar trebui să restaurați UPN original cu pașii din articol, [Restaurați un utilizator în Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="a8995-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="a8995-109">Dacă nu se poate restaura utilizatorul original ar trebui să eliminați utilizatorul vechi de pe site-ul OneDrive utilizând acești pași, [Eliminați un utilizator din lista de informații de utilizator]().</span><span class="sxs-lookup"><span data-stu-id="a8995-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="a8995-110">După aceasta se face, puteți verifica utilizatorul are drepturi de administrator pe site-ul OneDrive urmând pașii pentru a [adăuga admin pentru OneDrive unui utilizator](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="a8995-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="a8995-111">Pentru mai multe informații despre nivelurile de permisiune, consultați articolul, [Înțelegerea nivelurilor de permisiune în SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="a8995-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
