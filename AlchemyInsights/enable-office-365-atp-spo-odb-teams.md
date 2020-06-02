---
title: Activarea Office 365 ATP pentru SharePoint, OneDrive și Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506930"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="7b016-102">Activarea protecției avansate pentru amenințări Office 365 pentru SharePoint Online, OneDrive și Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7b016-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="7b016-103">Du-te https://protection.office.com și autentifică-te.</span><span class="sxs-lookup"><span data-stu-id="7b016-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="7b016-104">Alegeți **Threat management**  >  **Policy**  >  **Atașări sigure**pentru politica de gestionare a amenințărilor .</span><span class="sxs-lookup"><span data-stu-id="7b016-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="7b016-105">Selectați **Activare ATP pentru SharePoint, OneDrive și Microsoft Teams**, apoi faceți clic pe **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="7b016-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="7b016-106">(Recomandat) Ca administrator global sau administrator SharePoint Online, executați cmdletul [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cu parametrul **DisallowInfectedFileDownload** setat la *true*.</span><span class="sxs-lookup"><span data-stu-id="7b016-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="7b016-107">(Recomandat) [Configurați alerte](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pentru fișierele detectate.</span><span class="sxs-lookup"><span data-stu-id="7b016-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="7b016-108">ATP va scana fiecare fișier din SharePoint Online, OneDrive sau Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7b016-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="7b016-109">Fișierele sunt scanate asincron, printr-un proces care utilizează partajarea și evenimentele de activitate clienților, împreună cu euristica inteligentă și semnalele de amenințare pentru a identifica fișierele rău intenționate.</span><span class="sxs-lookup"><span data-stu-id="7b016-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="7b016-110">Consultați [ATP pentru SharePoint, OneDrive și Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="7b016-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>