---
title: Depanare acces refuzat mesaje OneDrive pentru afaceri site-uri
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232547"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="c6a57-102">Depanare acces refuzat mesaje OneDrive pentru afaceri site-uri</span><span class="sxs-lookup"><span data-stu-id="c6a57-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="c6a57-103">Această problemă apare cel mai frecvent atunci când un utilizator este şters şi re-creat cu acelaşi nume principal de utilizator (UPN).</span><span class="sxs-lookup"><span data-stu-id="c6a57-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="c6a57-104">Noul cont este creat folosind o valoare diferită de PUID (paşaport unic ID).</span><span class="sxs-lookup"><span data-stu-id="c6a57-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="c6a57-105">Atunci când utilizatorul încearcă să acceseze o colecţie de site-ul sau lor OneDrive, utilizatorul are un PUID incorecte.</span><span class="sxs-lookup"><span data-stu-id="c6a57-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="c6a57-106">Un al doilea scenariu implică sincronizare director cu o unitate organizaţională de Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="c6a57-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="c6a57-107">În cazul în care utilizatorii au deja conectat la SharePoint, apoi sa mutat la un OU diferite şi resynced cu SharePoint, acestea se pot confrunta aceasta problema.</span><span class="sxs-lookup"><span data-stu-id="c6a57-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="c6a57-108">Pentru a rezolva această problemă, ar trebui să restabiliţi UPN original cu paşii din articol,[restaura un utilizator în Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="c6a57-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="c6a57-109">În cazul în care nu se poate restabili original utilizator ar trebui să eliminaţi utilizatorul vechi din site-ul OneDrive folosind aceşti paşi, [elimina un utilizator din lista de informaţii utilizator]().</span><span class="sxs-lookup"><span data-stu-id="c6a57-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="c6a57-110">După ce acest lucru este făcut, puteţi verifica dacă utilizatorul are drepturi de administrator la site-ul OneDrive urmând paşii să [adăugaţi admin pe pentru un utilizator OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="c6a57-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="c6a57-111">Pentru mai multe informaţii despre nivelurile de permisiune, a se vedea articolul, [nivelurile de permisiune de înţelegere în SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="c6a57-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
