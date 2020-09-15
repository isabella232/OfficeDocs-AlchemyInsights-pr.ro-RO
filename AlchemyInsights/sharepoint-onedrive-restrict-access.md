---
title: Restricționarea accesului în SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700467"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="e3901-102">Restricționarea accesului în SharePoint sau OneDrive</span><span class="sxs-lookup"><span data-stu-id="e3901-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="e3901-103">Există mai multe modalități de a restricționa accesul la serviciile SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e3901-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="e3901-104">Aceste diverse metode de restricționare a accesului sunt prezentate mai jos.</span><span class="sxs-lookup"><span data-stu-id="e3901-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="e3901-105">**Restricție de permisiune**</span><span class="sxs-lookup"><span data-stu-id="e3901-105">**Permission Restriction**</span></span>

<span data-ttu-id="e3901-106">În SharePoint Online și OneDrive pentru Business, restricționăm accesul la elemente cum ar fi site-uri, fișiere și foldere prin acordarea accesului doar la acele grupuri/persoane care ar trebui să aibă acces.</span><span class="sxs-lookup"><span data-stu-id="e3901-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="e3901-107">Particularizarea permisiunilor pentru o listă sau o bibliotecă SharePoint</span><span class="sxs-lookup"><span data-stu-id="e3901-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="e3901-108">Particularizarea permisiunilor de site SharePoint</span><span class="sxs-lookup"><span data-stu-id="e3901-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="e3901-109">Modificarea permisiunilor pentru un subfolder</span><span class="sxs-lookup"><span data-stu-id="e3901-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="e3901-110">Controlul accesului de pe dispozitive negestionate</span><span class="sxs-lookup"><span data-stu-id="e3901-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="e3901-111">În calitate de administrator SharePoint sau global, puteți să blocați sau să limitați accesul la conținut SharePoint și OneDrive de pe dispozitive negestionate (acele reclame hibride care nu sunt asociate sau compatibile în Intune).</span><span class="sxs-lookup"><span data-stu-id="e3901-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="e3901-112">**Restricție de locație de rețea**</span><span class="sxs-lookup"><span data-stu-id="e3901-112">**Network Location Restriction**</span></span>

<span data-ttu-id="e3901-113">Ca administrator IT, puteți să controlați accesul la resursele SharePoint și OneDrive pe baza locațiilor de rețea definite în care aveți încredere.</span><span class="sxs-lookup"><span data-stu-id="e3901-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="e3901-114">Acest lucru este cunoscut și ca politică bazată pe locație.</span><span class="sxs-lookup"><span data-stu-id="e3901-114">This is also known as location-based policy.</span></span> <span data-ttu-id="e3901-115">Pentru mai multe informații, consultați [controlul accesului la date SharePoint Online și OneDrive pe baza locației rețelei](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="e3901-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="e3901-116">**Restricție de blocare a site-ului**</span><span class="sxs-lookup"><span data-stu-id="e3901-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="e3901-117">În SharePoint Online, aveți capacitatea de a bloca o colecție de site-uri, pentru ca nimeni să nu aibă acces.</span><span class="sxs-lookup"><span data-stu-id="e3901-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="e3901-118">Acest lucru este setat prin PowerShell și în [componenta de administrare SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) utilizând proprietatea [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="e3901-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="e3901-119">**Restricționarea utilizatorilor de la crearea de site-uri sau subsite-uri**</span><span class="sxs-lookup"><span data-stu-id="e3901-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="e3901-120">Ca administrator SharePoint sau administrator global, puteți permite utilizatorilor să creeze și să administreze propriile site-uri SharePoint, să stabilească ce tipuri de site-uri pot crea și să specifice locația site-urilor.</span><span class="sxs-lookup"><span data-stu-id="e3901-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="e3901-121">Pentru mai multe informații, consultați [gestionarea creării site-urilor în SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="e3901-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

