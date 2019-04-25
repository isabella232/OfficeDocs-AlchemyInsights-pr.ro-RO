---
title: Permite ATP Office 365 pentru SharePoint, OneDrive şi Microsoft echipe
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403045"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="69993-102">Activarea Office 365 ameninţare avansate de protecţie pentru SharePoint Online, OneDrive şi Microsoft echipe</span><span class="sxs-lookup"><span data-stu-id="69993-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="69993-103">Du-te la https://protection.office.com și conectați-vă.</span><span class="sxs-lookup"><span data-stu-id="69993-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="69993-104">Alege **Threat management** > **Politica** > **Atașări în condiţii de siguranţă**.</span><span class="sxs-lookup"><span data-stu-id="69993-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="69993-105">Selectați **activați ATP pentru SharePoint, OneDrive, şi echipe de Microsoft**, şi apoi faceţi clic pe **salvaţi**.</span><span class="sxs-lookup"><span data-stu-id="69993-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="69993-106">(Recomandat) Ca un administrator global sau un administrator de SharePoint Online, executaţi cmdlet-ul [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cu parametrul **DisallowInfectedFileDownload** setat la *adevărat*.</span><span class="sxs-lookup"><span data-stu-id="69993-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="69993-107">(Recomandat) [Configurarea avertizărilor](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pentru detectat fişierele.</span><span class="sxs-lookup"><span data-stu-id="69993-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="69993-108">ATP va nto scanare orice fişier în SharePoint Online, OneDrive sau Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="69993-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="69993-109">Fişierele sunt scanate asincron, printr-un proces care utilizează sharing şi comentariile evenimente activitatea, împreună cu smart euristică şi semnalele de ameninţare pentru a identifica fişierele rău intenţionat.</span><span class="sxs-lookup"><span data-stu-id="69993-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="69993-110">A se vedea [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="69993-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>