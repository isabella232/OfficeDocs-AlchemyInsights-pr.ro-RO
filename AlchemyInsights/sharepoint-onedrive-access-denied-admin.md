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
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505391"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="ddf51-102">Depanarea mesajelor refuzate de acces în Centrul de administrare Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="ddf51-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="ddf51-103">Dacă primiți un mesaj de acces refuzat atunci când încercați să navigați la un Centru de administrare Sharepoint/OneDrive, asigurați-vă că [atribuiți o licență utilizatorului](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="ddf51-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="ddf51-104">Dacă utilizatorul are o licență, trebuie să vă asigurați că li se [atribuie un rol de administrator](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) care poate accesa centrele de administrare.</span><span class="sxs-lookup"><span data-stu-id="ddf51-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="ddf51-105">Această problemă poate apărea, de asemenea, atunci când un utilizator este șters și recreat cu același nume principal de utilizator (UPN).</span><span class="sxs-lookup"><span data-stu-id="ddf51-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="ddf51-106">Noul cont este creat utilizând o valoare PUID (Passport Unique ID) diferită.</span><span class="sxs-lookup"><span data-stu-id="ddf51-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="ddf51-107">Când utilizatorul încearcă să acceseze o colecție de site-ul sau OneDrive lor, utilizatorul are un PUID incorecte.</span><span class="sxs-lookup"><span data-stu-id="ddf51-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="ddf51-108">Un al doilea scenariu implică sincronizarea directorului cu o unitate organizațională Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="ddf51-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="ddf51-109">Dacă utilizatorii s-au conectat deja la SharePoint, și apoi sunt mutate într-un alt OU și resynced cu SharePoint, acestea pot apărea această problemă.</span><span class="sxs-lookup"><span data-stu-id="ddf51-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="ddf51-110">Pentru a rezolva această problemă, ar trebui să restaurați UPN original cu pașii din articol, [Restaurați un utilizator în Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="ddf51-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="ddf51-111">Notă: Dacă un centru de administrare OneDrive sau SharePoint nu este disponibil pentru mai mulți utilizatori care au avut anterior acces, este posibil să existe o problemă de serviciu temporar.</span><span class="sxs-lookup"><span data-stu-id="ddf51-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="ddf51-112">[Verificați tabloul de bord de sănătate a serviciului](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="ddf51-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


