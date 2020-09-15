---
title: Depanarea mesajelor refuzate pentru site-urile OneDrive pentru Business
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670628"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="9eba2-102">Depanarea mesajelor refuzate pentru site-urile OneDrive pentru Business</span><span class="sxs-lookup"><span data-stu-id="9eba2-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="9eba2-103">Această problemă apare cel mai frecvent atunci când un utilizator este șters și creat din nou cu același nume principal de utilizator (UPN).</span><span class="sxs-lookup"><span data-stu-id="9eba2-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="9eba2-104">Noul cont este creat utilizând o altă valoare PUID (ID unic Passport).</span><span class="sxs-lookup"><span data-stu-id="9eba2-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="9eba2-105">Atunci când utilizatorul încearcă să acceseze o colecție de site-uri sau OneDrive, utilizatorul are o PUID incorectă.</span><span class="sxs-lookup"><span data-stu-id="9eba2-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="9eba2-106">Un al doilea scenariu implică sincronizarea directorului cu o unitate organizațională Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="9eba2-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="9eba2-107">Dacă utilizatorii s-au conectat deja la SharePoint, apoi sunt mutați la alt OU și Resincronizați cu SharePoint, este posibil ca aceștia să întâmpine această problemă.</span><span class="sxs-lookup"><span data-stu-id="9eba2-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="9eba2-108">Pentru a rezolva această problemă, trebuie să restaurați UPN-ul inițial cu pașii din articol, să [restaurați un utilizator în Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="9eba2-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="9eba2-109">Dacă nu puteți restaura utilizatorul inițial, ar trebui să eliminați utilizatorul vechi din site-ul OneDrive utilizând acești pași, să [Eliminați un utilizator din lista informații utilizator]().</span><span class="sxs-lookup"><span data-stu-id="9eba2-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="9eba2-110">După ce se termină acest lucru, puteți verifica dacă utilizatorul are drepturi de administrator la site-ul OneDrive, urmând pașii de [Adăugare a administratorului pentru OneDrive unui utilizator](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="9eba2-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="9eba2-111">Pentru mai multe informații despre nivelurile de permisiune, consultați articolul, [înțelegerea nivelurilor de permisiune din SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="9eba2-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
