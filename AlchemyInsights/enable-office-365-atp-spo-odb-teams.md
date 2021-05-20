---
title: Activarea Office 365 ATP pentru SharePoint, OneDrive și Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543940"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="27bf9-102">Activați Microsoft Defender pentru Office 365 pentru SharePoint Online, pentru OneDrive, pentru Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="27bf9-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="27bf9-103">Mergeți https://protection.office.com la și conectați-vă.</span><span class="sxs-lookup"><span data-stu-id="27bf9-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="27bf9-104">Alegeți **Politică de gestionare** a  >    >  **amenințărilor Seif Atașări.**</span><span class="sxs-lookup"><span data-stu-id="27bf9-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="27bf9-105">Selectați **Activați Defender pentru Office 365 pentru SharePoint, OneDrive și Microsoft Teams**, apoi faceți clic pe **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="27bf9-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="27bf9-106">(Recomandat) Ca administrator global sau administrator SharePoint Online, rulați cmdletul [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cu **DisallowInfectedFileDownload** parametrul setat la *true*.</span><span class="sxs-lookup"><span data-stu-id="27bf9-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="27bf9-107">(Recomandat) [Configurați avertizările](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pentru fișierele detectate.</span><span class="sxs-lookup"><span data-stu-id="27bf9-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="27bf9-108">Microsoft Defender pentru Office 365 va scana fiecare fișier în SharePoint Online, OneDrive sau Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="27bf9-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="27bf9-109">Fișierele sunt scanate asincron, printr-un proces care utilizează evenimente de partajare și de activitate a invitaților, împreună cu o heuristică inteligentă și semnale de amenințare pentru a identifica fișierele rău intenționate.</span><span class="sxs-lookup"><span data-stu-id="27bf9-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="27bf9-110">Consultați [Microsoft Defender pentru Office 365 pentru SharePoint, OneDrive, apoi Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="27bf9-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>