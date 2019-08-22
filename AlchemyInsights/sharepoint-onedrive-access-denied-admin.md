---
title: Depanați mesajele de acces refuzat
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503548"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="3f24e-102">Depanarea Access Denied mesaje în centrul de administrare Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="3f24e-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="3f24e-103">Dacă vi se administrează un accent denied mesaj atunci când încearcă să navigaţi la un centru de administrare Sharepoint/OneDrive, vă rugăm să asiguraţi-vă că vă [atribuiţi o licenţă de utilizator](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="3f24e-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="3f24e-104">În cazul în care utilizatorul are o licenta, de asemenea, ar trebui să asiguraţi-vă că acestea se [atribuie un rol de administrator](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) care poate accesa centrele de admin.</span><span class="sxs-lookup"><span data-stu-id="3f24e-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="3f24e-105">Această problemă poate apărea când un utilizator este şters şi re-creat cu acelaşi nume principal de utilizator (UPN).</span><span class="sxs-lookup"><span data-stu-id="3f24e-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="3f24e-106">Noul cont este creat folosind o valoare diferită de PUID (paşaport unic ID).</span><span class="sxs-lookup"><span data-stu-id="3f24e-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="3f24e-107">Atunci când utilizatorul încearcă să acceseze o colecţie de site-ul sau lor OneDrive, utilizatorul are un PUID incorecte.</span><span class="sxs-lookup"><span data-stu-id="3f24e-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="3f24e-108">Un al doilea scenariu implică sincronizare director cu o unitate organizaţională de Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="3f24e-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="3f24e-109">În cazul în care utilizatorii au deja conectat la SharePoint, apoi sa mutat la un OU diferite şi resynced cu SharePoint, acestea se pot confrunta aceasta problema.</span><span class="sxs-lookup"><span data-stu-id="3f24e-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="3f24e-110">Pentru a rezolva această problemă, trebuie să restabiliţi UPN original cu paşii din articol, [restaura un utilizator în Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="3f24e-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="3f24e-111">Notă: În cazul în care un centru de OneDrive sau administrator SharePoint nu este disponibil pentru mai mulţi utilizatori care anterior a avut acces, poate fi o problemă temporară serviciu.</span><span class="sxs-lookup"><span data-stu-id="3f24e-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="3f24e-112">[Verificaţi tabloul de sănătate serviciu](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="3f24e-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


