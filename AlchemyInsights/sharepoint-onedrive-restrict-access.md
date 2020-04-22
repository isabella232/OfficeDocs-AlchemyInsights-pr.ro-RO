---
title: Restricționarea accesului în SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692777"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="c91bf-102">Restricționarea accesului în SharePoint sau OneDrive</span><span class="sxs-lookup"><span data-stu-id="c91bf-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="c91bf-103">Există multe modalități de a restricționa accesul la serviciile SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c91bf-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="c91bf-104">Aceste diferite metode de restricționare a accesului sunt prezentate mai jos.</span><span class="sxs-lookup"><span data-stu-id="c91bf-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="c91bf-105">**Restricționare permisiune**</span><span class="sxs-lookup"><span data-stu-id="c91bf-105">**Permission Restriction**</span></span>

<span data-ttu-id="c91bf-106">În SharePoint Online și OneDrive for Business, restricționăm accesul la elemente precum site-uri, fișiere și foldere, acordând acces numai la acele grupuri/persoane care ar trebui să aibă acces.</span><span class="sxs-lookup"><span data-stu-id="c91bf-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="c91bf-107">Particularizarea permisiunilor pentru o listă sau o bibliotecă SharePoint</span><span class="sxs-lookup"><span data-stu-id="c91bf-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="c91bf-108">Particularizarea permisiunilor de site SharePoint</span><span class="sxs-lookup"><span data-stu-id="c91bf-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="c91bf-109">Modificarea permisiunilor pentru un subfolder</span><span class="sxs-lookup"><span data-stu-id="c91bf-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="c91bf-110">Controlul accesului de la dispozitive negestionate</span><span class="sxs-lookup"><span data-stu-id="c91bf-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="c91bf-111">Ca administrator SharePoint sau global, puteți bloca sau limita accesul la conținutul SharePoint și OneDrive de pe dispozitive negestionate (cele care nu sunt asociate sau conforme cu AD hibrid în Intune).</span><span class="sxs-lookup"><span data-stu-id="c91bf-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="c91bf-112">**Restricționare locație rețea**</span><span class="sxs-lookup"><span data-stu-id="c91bf-112">**Network Location Restriction**</span></span>

<span data-ttu-id="c91bf-113">Ca administrator IT, puteți controla accesul la resursele SharePoint și OneDrive pe baza locațiilor de rețea definite în care aveți încredere.</span><span class="sxs-lookup"><span data-stu-id="c91bf-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="c91bf-114">Aceasta este cunoscută și sub numele de politică bazată pe locație.</span><span class="sxs-lookup"><span data-stu-id="c91bf-114">This is also known as location-based policy.</span></span> <span data-ttu-id="c91bf-115">Pentru mai multe informații, consultați [Controlul accesului la datele SharePoint Online și OneDrive bazate pe locația de rețea](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="c91bf-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="c91bf-116">**Restricționare blocare site**</span><span class="sxs-lookup"><span data-stu-id="c91bf-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="c91bf-117">În SharePoint Online aveți posibilitatea de a bloca o colecție de site-uri, astfel încât nimeni să nu aibă acces.</span><span class="sxs-lookup"><span data-stu-id="c91bf-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="c91bf-118">Acest lucru este setată prin PowerShell și [Componentă de administrare SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) utilizând proprietatea [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.</span><span class="sxs-lookup"><span data-stu-id="c91bf-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="c91bf-119">**Restricționarea utilizatorilor de la crearea de site-uri sau subsite-uri**</span><span class="sxs-lookup"><span data-stu-id="c91bf-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="c91bf-120">Ca administrator SharePoint sau administrator global, puteți permite utilizatorilor să creeze și să administreze propriile site-uri SharePoint, să determine ce fel de site-uri pot crea și să specificați locația site-urilor.</span><span class="sxs-lookup"><span data-stu-id="c91bf-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="c91bf-121">Pentru mai multe informații, consultați [Gestionarea creării site-ului în SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="c91bf-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

