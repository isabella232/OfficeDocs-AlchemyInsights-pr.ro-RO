---
title: Probleme de conexiune SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508435"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="fa12e-102">Probleme de conexiune SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="fa12e-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="fa12e-103">În cazul în care SharePoint Designer se confruntă cu probleme de conectare la site-uri SharePoint, încercați următoarele soluții comune.</span><span class="sxs-lookup"><span data-stu-id="fa12e-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="fa12e-104">Pasul 1: Verificaţi că SharePoint Designer 2013 este actualizat cu [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) şi [2 august 2016 Update pentru SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="fa12e-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="fa12e-105">Pasul 2: Şterge fişierele cache-ul local:</span><span class="sxs-lookup"><span data-stu-id="fa12e-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="fa12e-106">Închide SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="fa12e-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="fa12e-107">Pe computerul local, eliminaţi toate fişierele găsite în fiecare din următoarele foldere.</span><span class="sxs-lookup"><span data-stu-id="fa12e-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="fa12e-108">%AppData%\Microsoft\Web server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="fa12e-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="fa12e-109">%AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="fa12e-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="fa12e-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="fa12e-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="fa12e-111">Deschide SharePoint Designer 2013 şi introduceţi contul din nou pentru a vedea dacă funcţionează.</span><span class="sxs-lookup"><span data-stu-id="fa12e-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="fa12e-112">Pasul 3: [activa autentificarea moderne pentru Office 2013 pe Windows dispozitive](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="fa12e-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="fa12e-113">Pasul 4: Administratorii va trebui să **Permite script-ul personalizat** în setările de centru de administrare SharePoint pentru a permite conexiunea de SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="fa12e-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="fa12e-114">Vedea [permite sau împiedică script-ul personalizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) pentru mai multe informaţii.</span><span class="sxs-lookup"><span data-stu-id="fa12e-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


