---
title: Restricționați accesul în SharePoint sau OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750676"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="38fab-102">Restricționați accesul în SharePoint sau OneDrive</span><span class="sxs-lookup"><span data-stu-id="38fab-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="38fab-103">Există multe modalități de a restricționa accesul la serviciile SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="38fab-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="38fab-104">Aceste diferite metode de restricționare a accesului sunt prezentate mai jos.</span><span class="sxs-lookup"><span data-stu-id="38fab-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="38fab-105">**Restricție permisiune**</span><span class="sxs-lookup"><span data-stu-id="38fab-105">**Permission Restriction**</span></span>

<span data-ttu-id="38fab-106">În SharePoint Online și OneDrive for Business, restricționăm accesul la elemente ar fi site-uri, fișiere și foldere prin acordarea accesului numai la acele grupuri/persoane care ar trebui să aibă acces.</span><span class="sxs-lookup"><span data-stu-id="38fab-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="38fab-107">Particularizarea permisiunilor pentru o listă sau o bibliotecă SharePoint</span><span class="sxs-lookup"><span data-stu-id="38fab-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="38fab-108">Particularizarea permisiunilor de site SharePoint</span><span class="sxs-lookup"><span data-stu-id="38fab-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="38fab-109">Modificarea permisiunilor unui subfolder</span><span class="sxs-lookup"><span data-stu-id="38fab-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="38fab-110">Controlul accesului de la dispozitive negestionate</span><span class="sxs-lookup"><span data-stu-id="38fab-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="38fab-111">Ca un SharePoint sau Global admin în Office 365, aveți posibilitatea să blocați sau să limitați accesul la conținut SharePoint și OneDrive de pe dispozitive negestionate (cei care nu hibrid AD alăturat sau conforme în Intune).</span><span class="sxs-lookup"><span data-stu-id="38fab-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="38fab-112">**Restricție Locație rețea**</span><span class="sxs-lookup"><span data-stu-id="38fab-112">**Network Location Restriction**</span></span>

<span data-ttu-id="38fab-113">Ca administrator IT, puteți controla accesul la resursele SharePoint și OneDrive pe baza unor locații de rețea definite în care aveți încredere.</span><span class="sxs-lookup"><span data-stu-id="38fab-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="38fab-114">Acest lucru este cunoscut și ca politică bazată pe locație.</span><span class="sxs-lookup"><span data-stu-id="38fab-114">This is also known as location-based policy.</span></span> <span data-ttu-id="38fab-115">Pentru mai multe informații, consultați [controlul accesului la datele SharePoint Online și OneDrive bazate pe locația de rețea](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="38fab-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="38fab-116">**Restricționare blocare site**</span><span class="sxs-lookup"><span data-stu-id="38fab-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="38fab-117">În SharePoint Online aveți posibilitatea de a bloca o colecție de site-uri, astfel încât nimeni nu are acces.</span><span class="sxs-lookup"><span data-stu-id="38fab-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="38fab-118">Acest lucru este setat prin PowerShell și [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) utilizând proprietatea [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="38fab-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="38fab-119">**Restricționarea utilizatorilor de crearea de site-uri sau subsite-uri**</span><span class="sxs-lookup"><span data-stu-id="38fab-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="38fab-120">Ca administrator SharePoint sau Office 365 global admin, puteți lăsa utilizatorii să creeze și să administreze propriile site-uri SharePoint, să determine ce fel de site-uri pot crea și să precizeze locația site-urilor.</span><span class="sxs-lookup"><span data-stu-id="38fab-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="38fab-121">Pentru mai multe informații, consultați [gestionarea creării site-ului în SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="38fab-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

