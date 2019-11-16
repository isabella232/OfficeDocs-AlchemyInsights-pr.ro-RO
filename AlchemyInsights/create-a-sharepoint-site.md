---
title: Crearea unui sit SharePoint
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ac894195d847dfc009bc0b57647e1a474361f1c1
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769603"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="ee34f-102">Crearea unui sit SharePoint</span><span class="sxs-lookup"><span data-stu-id="ee34f-102">Create a SharePoint site</span></span>

<span data-ttu-id="ee34f-103">Puteți vedea următoarele informații despre crearea de site-uri SharePoint:</span><span class="sxs-lookup"><span data-stu-id="ee34f-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="ee34f-104">[Gestionați site-uri în noul centru de administrare SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): Aflați despre opțiunile de creare a site-ului, inclusiv despre se creează un site clasic sau un site de echipe care nu include un grup Office 365.</span><span class="sxs-lookup"><span data-stu-id="ee34f-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="ee34f-105">[Creați un site de echipă în SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Aflați să creați un site de echipă.</span><span class="sxs-lookup"><span data-stu-id="ee34f-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="ee34f-106">[Creați un site de comunicare în SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Aflați să creați un site de comunicații.</span><span class="sxs-lookup"><span data-stu-id="ee34f-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="ee34f-107">[Gestionați site-uri în noul centru de administrare SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Aflați să creați un site clasic sau un site de echipă care nu include un grup Office 365.</span><span class="sxs-lookup"><span data-stu-id="ee34f-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
<span data-ttu-id="ee34f-108">**Sfaturi:**</span><span class="sxs-lookup"><span data-stu-id="ee34f-108">**Tips:**</span></span>
- <span data-ttu-id="ee34f-109">Imposibil de creat un site cu același URL al unui site existent.</span><span class="sxs-lookup"><span data-stu-id="ee34f-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="ee34f-110">Dacă ați șters un site și doriți să reutilizați adresa URL, este posibil ca site-ul șters să existe în continuare sub **site-uri șterse**.</span><span class="sxs-lookup"><span data-stu-id="ee34f-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="ee34f-111">Pentru a gestiona site-urile șterse, consultați, [Ștergeți un site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="ee34f-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="ee34f-112">Pentru a elimina complet un site cu PowerShell, consultați exemplu cmdletul [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="ee34f-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="ee34f-113">Este posibil ca unii utilizatori să nu poată crea un site.</span><span class="sxs-lookup"><span data-stu-id="ee34f-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="ee34f-114">Consultați [gestionarea creării site-ului în SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="ee34f-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="ee34f-115">Este posibil site-ul apare blocat la **crearea** mai mult decât se aștepta.</span><span class="sxs-lookup"><span data-stu-id="ee34f-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="ee34f-116">Dacă au trecut mai mult de 24 de ore de când ați văzut prima dată această problemă, vă rugăm să înregistrați un bilet de suport.</span><span class="sxs-lookup"><span data-stu-id="ee34f-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="ee34f-117">În multe cazuri, suntem deja de lucru pe o soluție.</span><span class="sxs-lookup"><span data-stu-id="ee34f-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="ee34f-118">Vă rugăm să ne acordați cel puțin 24 de ore pentru a finaliza o soluție.</span><span class="sxs-lookup"><span data-stu-id="ee34f-118">Please give us at least 24 hours to complete a solution.</span></span>
- <span data-ttu-id="ee34f-119">Dacă trebuie să creați un nou site de echipă care nu include un grup Office 365,</span><span class="sxs-lookup"><span data-stu-id="ee34f-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


