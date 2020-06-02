---
title: Probleme de conexiune SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511556"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="b826b-102">Probleme de conexiune SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="b826b-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="b826b-103">Dacă SharePoint Designer întâmpină probleme de conexiune la site-urile SharePoint, încercați următoarele soluții comune.</span><span class="sxs-lookup"><span data-stu-id="b826b-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="b826b-104">Pasul 1: Verificați că SharePoint Designer 2013 este actualizat cu [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) și actualizarea 2 August [2016 pentru SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="b826b-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="b826b-105">Pasul 2: Goliți fișierele cache locale:</span><span class="sxs-lookup"><span data-stu-id="b826b-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="b826b-106">Închideți SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="b826b-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="b826b-107">Pe computerul local, eliminați toate fișierele găsite în fiecare dintre următoarele foldere.</span><span class="sxs-lookup"><span data-stu-id="b826b-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="b826b-108">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\Web Server Extensions\Cache %APP</span><span class="sxs-lookup"><span data-stu-id="b826b-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="b826b-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="b826b-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="b826b-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="b826b-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="b826b-111">Deschideți SharePoint Designer 2013 și introduceți din nou contul pentru a vedea dacă funcționează.</span><span class="sxs-lookup"><span data-stu-id="b826b-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="b826b-112">Pasul 3: [Activați autentificarea modernă pentru Office 2013 pe dispozitive Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="b826b-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="b826b-113">Pasul 4: Administratorii vor trebui să **permită scriptul personalizat** în setările Centrului de administrare SharePoint pentru a permite conexiunea SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="b826b-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="b826b-114">Consultați [Permiterea sau împiedicarea scriptului particularizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="b826b-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


