---
title: Clientul Teams are căderi?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826283"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="71fc2-102">Clientul Teams are căderi?</span><span class="sxs-lookup"><span data-stu-id="71fc2-102">Teams client crashing?</span></span>

<span data-ttu-id="71fc2-103">Dacă clientul dvs. Teams are căderi, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="71fc2-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="71fc2-104">Dacă utilizați aplicația desktop Teams, [asigurați-vă că aplicația este complet actualizată](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="71fc2-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="71fc2-105">Asigurați-vă că toate adresele URL și intervalele de adrese [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) sunt accesibile.</span><span class="sxs-lookup"><span data-stu-id="71fc2-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="71fc2-106">Conectați-vă cu contul de administrator al entității găzduite și verificați tabloul de bord [cu](https://docs.microsoft.com/office365/enterprise/view-service-health) starea serviciilor pentru a verifica dacă nu există nicio degradare sau degradare a serviciului.</span><span class="sxs-lookup"><span data-stu-id="71fc2-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="71fc2-107">Dezinstalați și reinstalați aplicația Teams (link)</span><span class="sxs-lookup"><span data-stu-id="71fc2-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="71fc2-108">Navigați la folderul %appdata%\Microsoft\teams\ de pe computer și ștergeți toate fișierele din acel director.</span><span class="sxs-lookup"><span data-stu-id="71fc2-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="71fc2-109">[Descărcați și instalați aplicația Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), iar dacă este posibil, instalați Teams ca administrator (dați clic dreapta pe programul de instalare Teams și selectați "Rulați ca administrator", dacă este disponibil).</span><span class="sxs-lookup"><span data-stu-id="71fc2-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="71fc2-110">În cazul în care clientul dvs. Teams are în continuare probleme, puteți reproduce problema?</span><span class="sxs-lookup"><span data-stu-id="71fc2-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="71fc2-111">Dacă da:</span><span class="sxs-lookup"><span data-stu-id="71fc2-111">If so:</span></span>

1. <span data-ttu-id="71fc2-112">Utilizați înregistratorul de pași pentru a captura pașii.</span><span class="sxs-lookup"><span data-stu-id="71fc2-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="71fc2-113">Închideți TOATE aplicațiile inutile sau confidențiale.</span><span class="sxs-lookup"><span data-stu-id="71fc2-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="71fc2-114">Lansați înregistratorul de pași și reproduceți problema în timp ce sunteți conectat cu contul de utilizator afectat.</span><span class="sxs-lookup"><span data-stu-id="71fc2-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="71fc2-115">[Colectați jurnalele echipelor care capturează pașii de repro înregistrate.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="71fc2-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="71fc2-116">**Notă:** Asigurați-vă că capturați adresa de conectare a utilizatorului afectat.</span><span class="sxs-lookup"><span data-stu-id="71fc2-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="71fc2-117">Colectați e-mailul și/sau informațiile despre bucketul de eroare (Windows).</span><span class="sxs-lookup"><span data-stu-id="71fc2-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="71fc2-118">Lansați windows Powershell pe computerul pe care are loc căderea și rulați următoarele comenzi:</span><span class="sxs-lookup"><span data-stu-id="71fc2-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="71fc2-119">Atașați fișierul la cazul dvs. de asistență.</span><span class="sxs-lookup"><span data-stu-id="71fc2-119">Attach the file to your support case.</span></span>
