---
title: Clientul Teams are căderi?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354064"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="7dfd9-102">Clientul Teams are căderi?</span><span class="sxs-lookup"><span data-stu-id="7dfd9-102">Teams client crashing?</span></span>

<span data-ttu-id="7dfd9-103">Dacă clientul dvs. Teams are căderi, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="7dfd9-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="7dfd9-104">Dacă utilizați aplicația desktop Teams, [asigurați-vă că aplicația este complet actualizată](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="7dfd9-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="7dfd9-105">Asigurați-vă că toate [adresele URL Microsoft 365 și intervalele de adrese](https://docs.microsoft.com/microsoftteams/connectivity-issues) sunt accesibile.</span><span class="sxs-lookup"><span data-stu-id="7dfd9-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="7dfd9-106">Conectați-vă cu contul de administrator al entității găzduite și verificați [Tabloul de bord de sănătate serviciu](https://docs.microsoft.com/office365/enterprise/view-service-health) pentru a verifica dacă nu există nicio întrerupere sau degradare a serviciului.</span><span class="sxs-lookup"><span data-stu-id="7dfd9-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="7dfd9-107">Dezinstalarea și reinstalarea aplicației Teams (link)</span><span class="sxs-lookup"><span data-stu-id="7dfd9-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="7dfd9-108">Navigați la folderul %appdata%\Microsoft\teams\ de pe computer și ștergeți toate fișierele din acel director.</span><span class="sxs-lookup"><span data-stu-id="7dfd9-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="7dfd9-109">[Descărcați și instalați aplicația Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)și, dacă este posibil, instalați Teams ca administrator (faceți clic dreapta pe programul de instalare Teams și selectați "Executare ca administrator", dacă este disponibil).</span><span class="sxs-lookup"><span data-stu-id="7dfd9-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="7dfd9-110">Dacă clientul tău Teams încă se prăbușește, poți reproduce problema?</span><span class="sxs-lookup"><span data-stu-id="7dfd9-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="7dfd9-111">Dacă da:</span><span class="sxs-lookup"><span data-stu-id="7dfd9-111">If so:</span></span>

1. <span data-ttu-id="7dfd9-112">Utilizați Înregistratorul de pași pentru a captura pașii.</span><span class="sxs-lookup"><span data-stu-id="7dfd9-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="7dfd9-113">Închideți toate aplicațiile inutile sau confidențiale.</span><span class="sxs-lookup"><span data-stu-id="7dfd9-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="7dfd9-114">Lansați Înregistratorul de pași și reproduceți problema în timp ce faceți Log in cu contul de utilizator afectat.</span><span class="sxs-lookup"><span data-stu-id="7dfd9-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="7dfd9-115">[Colecta jurnalele de echipe care captează pașii de repro înregistrate](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="7dfd9-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="7dfd9-116">**Notă:** Asigurați-vă că capturați adresa de conectare a utilizatorului afectat.</span><span class="sxs-lookup"><span data-stu-id="7dfd9-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="7dfd9-117">Colectați informațiile despre dump și/sau din găleata de defecte (Windows).</span><span class="sxs-lookup"><span data-stu-id="7dfd9-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="7dfd9-118">Lansarea Windows Powershell pe computerul în cazul în care se produce accident și executați următoarele comenzi:</span><span class="sxs-lookup"><span data-stu-id="7dfd9-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="7dfd9-119">Atașați fișierul la cazul de asistență.</span><span class="sxs-lookup"><span data-stu-id="7dfd9-119">Attach the file to your support case.</span></span>
