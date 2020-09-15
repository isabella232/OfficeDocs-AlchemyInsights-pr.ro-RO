---
title: Activarea Office 365 ATP pentru SharePoint, OneDrive și Microsoft teams
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709919"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="5a2c1-102">Activarea protecției avansate a amenințărilor Office 365 pentru SharePoint Online, OneDrive și Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="5a2c1-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="5a2c1-103">Accesați https://protection.office.com și conectați-vă.</span><span class="sxs-lookup"><span data-stu-id="5a2c1-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="5a2c1-104">Alegeți Politica de **gestionare a amenințărilor**  >  **Policy**  >  **atașări sigure**.</span><span class="sxs-lookup"><span data-stu-id="5a2c1-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="5a2c1-105">Selectați **activați ATP pentru SharePoint, OneDrive și Microsoft teams**, apoi faceți clic pe **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="5a2c1-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="5a2c1-106">Recomandate Ca administrator global sau administrator SharePoint Online, rulează cmdletul [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cu parametrul **DisallowInfectedFileDownload** setat la *True*.</span><span class="sxs-lookup"><span data-stu-id="5a2c1-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="5a2c1-107">Recomandate [Configurați avertizări](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pentru fișierele detectate.</span><span class="sxs-lookup"><span data-stu-id="5a2c1-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="5a2c1-108">ATP va scana fiecare fișier din SharePoint Online, OneDrive sau Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="5a2c1-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="5a2c1-109">Fișierele sunt scanate asincron, printr-un proces care utilizează evenimente de partajare și de activitate ale invitaților, împreună cu euristica inteligentă și semnalele de amenințare pentru a identifica fișiere periculoase.</span><span class="sxs-lookup"><span data-stu-id="5a2c1-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="5a2c1-110">Consultați [ATP pentru SharePoint, OneDrive și Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="5a2c1-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>