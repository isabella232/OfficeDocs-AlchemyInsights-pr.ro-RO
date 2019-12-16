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
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051437"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="01e79-102">Depanarea mesajelor de acces refuzat în SharePoint/OneDrive Admin Center</span><span class="sxs-lookup"><span data-stu-id="01e79-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="01e79-103">Dacă primiți un mesaj de acces refuzat atunci când încercați să navigați la un centru de administrare SharePoint/OneDrive, asigurați-vă că [atribuiți o licență pentru utilizator](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="01e79-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="01e79-104">Dacă utilizatorul are o licență, de asemenea, trebuie să vă asigurați că sunt [atribuite un rol de administrator](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) care pot accesa centrele de administrare.</span><span class="sxs-lookup"><span data-stu-id="01e79-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="01e79-105">Această problemă poate apărea, de asemenea, atunci când un utilizator este șters și re-creat cu același nume principal de utilizator (UPN).</span><span class="sxs-lookup"><span data-stu-id="01e79-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="01e79-106">Noul cont este creat utilizând un alt PUID (pașaport Unique ID) valoare.</span><span class="sxs-lookup"><span data-stu-id="01e79-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="01e79-107">Când utilizatorul încearcă să acceseze o colecție de site-uri sau OneDrive lor, utilizatorul are un PUID incorect.</span><span class="sxs-lookup"><span data-stu-id="01e79-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="01e79-108">Un al doilea scenariu implică sincronizare director cu o unitate organizațională Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="01e79-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="01e79-109">Dacă utilizatorii s-au conectat deja la SharePoint și apoi sunt mutate într-un ou diferit și traducerea cu SharePoint, acestea pot experimenta această problemă.</span><span class="sxs-lookup"><span data-stu-id="01e79-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="01e79-110">Pentru a rezolva această problemă, ar trebui să restaurați UPN originală cu pașii din articol, [restaurați un utilizator în Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="01e79-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="01e79-111">Notă: dacă un centru de administrare OneDrive sau SharePoint nu este disponibil pentru mai mulți utilizatori care au avut anterior acces, poate exista o problemă de serviciu temporar.</span><span class="sxs-lookup"><span data-stu-id="01e79-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="01e79-112">[Verificați tabloul de bord de sănătate Service](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="01e79-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


