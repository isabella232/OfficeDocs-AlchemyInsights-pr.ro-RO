---
title: Depanarea performanței OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757897"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="25b4b-102">Depanarea performanței OneDrive</span><span class="sxs-lookup"><span data-stu-id="25b4b-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="25b4b-103">Dacă întâmpinați o sincronizare mai lentă decât cea așteptată sau probleme de performanță similare cu OneDrive:</span><span class="sxs-lookup"><span data-stu-id="25b4b-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="25b4b-104">Confirmați că nu există probleme cunoscute utilizând [tabloul de bord stare servicii](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="25b4b-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="25b4b-105">[Activați fișierele la cerere](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) , astfel încât să vă puteți accesa toate fișierele din OneDrive fără a fi necesar să le descărcați pe toate și să utilizați spațiul de stocare pe dispozitivul dvs.</span><span class="sxs-lookup"><span data-stu-id="25b4b-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="25b4b-106">[Revizuiți cele mai bune practici](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) pentru planificarea și performanța rețelei.</span><span class="sxs-lookup"><span data-stu-id="25b4b-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="25b4b-107">[Maximizați viteza de încărcare și descărcare](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), mai ales dacă sincronizați pentru prima dată un dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="25b4b-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="25b4b-108">Dacă sincronizați o bibliotecă cu mai mult de 100.000 de elemente, sincronizarea OneDrive poate părea blocată mult timp sau starea afișează 0KB de procesare a xMB. "</span><span class="sxs-lookup"><span data-stu-id="25b4b-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="25b4b-109">[Aflați mai multe despre sincronizarea mai multor fișiere 100.000](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) , precum și [a limitei de 300.000 a fișierelor acceptate de OneDrive](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="25b4b-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="25b4b-110">Atunci când un utilizator depășește limitele de utilizare, SharePoint Online accelerează orice solicitări ulterioare din acel cont de utilizator pentru o perioadă scurtă de timp.</span><span class="sxs-lookup"><span data-stu-id="25b4b-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="25b4b-111">Toate acțiunile utilizatorilor sunt accelerați în timp ce acceleratorul este în vigoare.</span><span class="sxs-lookup"><span data-stu-id="25b4b-111">All user actions are throttled while the throttle is in effect.</span></span>
