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
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707966"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="6a4d6-102">Depanarea mesajelor refuzate în centrul de administrare SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="6a4d6-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="6a4d6-103">Dacă primiți un mesaj de acces refuzat atunci când încercați să navigați la un centru de administrare SharePoint/OneDrive, asigurați-vă că [atribuiți o licență pentru utilizator](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="6a4d6-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="6a4d6-104">Dacă utilizatorul are o licență, trebuie, de asemenea, să vă asigurați că i se [atribuie un rol de administrator](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) care poate accesa centrele de administrare.</span><span class="sxs-lookup"><span data-stu-id="6a4d6-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="6a4d6-105">Această problemă poate apărea și atunci când un utilizator este șters și recreat cu același nume principal de utilizator (UPN).</span><span class="sxs-lookup"><span data-stu-id="6a4d6-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="6a4d6-106">Noul cont este creat utilizând o altă valoare PUID (ID unic Passport).</span><span class="sxs-lookup"><span data-stu-id="6a4d6-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="6a4d6-107">Atunci când utilizatorul încearcă să acceseze o colecție de site-uri sau OneDrive, utilizatorul are o PUID incorectă.</span><span class="sxs-lookup"><span data-stu-id="6a4d6-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="6a4d6-108">Un al doilea scenariu implică sincronizarea directorului cu o unitate organizațională Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="6a4d6-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="6a4d6-109">Dacă utilizatorii s-au conectat deja la SharePoint, apoi sunt mutați la alt OU și Resincronizați cu SharePoint, este posibil ca aceștia să întâmpine această problemă.</span><span class="sxs-lookup"><span data-stu-id="6a4d6-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="6a4d6-110">Pentru a rezolva această problemă, trebuie să restaurați UPN-ul inițial cu pașii din articol, să [restaurați un utilizator în Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="6a4d6-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="6a4d6-111">Notă: dacă un centru de administrare OneDrive sau SharePoint nu este disponibil pentru mai mulți utilizatori care au avut acces anterior, este posibil să existe o problemă de serviciu temporară.</span><span class="sxs-lookup"><span data-stu-id="6a4d6-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="6a4d6-112">[Verificați tabloul de bord pentru starea serviciilor](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="6a4d6-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


