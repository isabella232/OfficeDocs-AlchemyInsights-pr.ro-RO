---
title: Teams client care se blochează
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187733"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="7faaf-102">Teams client care se blochează</span><span class="sxs-lookup"><span data-stu-id="7faaf-102">Teams client crashing</span></span>

<span data-ttu-id="7faaf-103">Dacă clientul dvs. Teams are căderi, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="7faaf-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="7faaf-104">Dacă utilizați aplicația desktop Teams, [asigurați-vă că aplicația este complet actualizată](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="7faaf-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="7faaf-105">Asigurați-vă că [toate adresele URL Microsoft 365 adresele URL și intervalele de](/microsoftteams/connectivity-issues) adrese sunt accesibile.</span><span class="sxs-lookup"><span data-stu-id="7faaf-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="7faaf-106">Conectați-vă cu contul de administrator al entității găzduite și verificați tabloul de bord [cu](/office365/enterprise/view-service-health) starea serviciilor pentru a verifica dacă nu există nicio degradare sau degradare a serviciului.</span><span class="sxs-lookup"><span data-stu-id="7faaf-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="7faaf-107">Dezinstalarea și reinstalarea aplicației Teams Software</span><span class="sxs-lookup"><span data-stu-id="7faaf-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="7faaf-108">Navigați la folderul %appdata%\Microsoft\Teams\ de pe computer și ștergeți toate fișierele din acel director.</span><span class="sxs-lookup"><span data-stu-id="7faaf-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="7faaf-109">[Descărcați](https://www.microsoft.com/microsoft-teams/download-app)și instalați aplicația Teams și, dacă este posibil, instalați Teams ca administrator (faceți clic dreapta pe programul de instalare Teams și selectați Executare ca **administrator,** dacă este disponibil).</span><span class="sxs-lookup"><span data-stu-id="7faaf-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="7faaf-110">Dacă clientul Teams încă se blochează, încercați să reproduceți problema.</span><span class="sxs-lookup"><span data-stu-id="7faaf-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="7faaf-111">Dacă puteți:</span><span class="sxs-lookup"><span data-stu-id="7faaf-111">If you can:</span></span>

1. <span data-ttu-id="7faaf-112">Utilizați înregistratorul de pași pentru a captura pașii.</span><span class="sxs-lookup"><span data-stu-id="7faaf-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="7faaf-113">Închideți TOATE aplicațiile inutile sau confidențiale.</span><span class="sxs-lookup"><span data-stu-id="7faaf-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="7faaf-114">Lansați înregistratorul de pași și reproduceți problema în timp ce sunteți conectat cu contul de utilizator afectat.</span><span class="sxs-lookup"><span data-stu-id="7faaf-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="7faaf-115">[Colectați jurnalele echipelor care capturează pașii de repro înregistrate.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="7faaf-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="7faaf-116">**Notă:** Asigurați-vă că capturați adresa de conectare a utilizatorului afectat.</span><span class="sxs-lookup"><span data-stu-id="7faaf-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="7faaf-117">Colectați informațiile despre defecțiuni și/sau despre bucketul de eroare (Windows).</span><span class="sxs-lookup"><span data-stu-id="7faaf-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="7faaf-118">Lansați Windows Powershell pe computerul pe care are loc căderea și rulați următoarele comenzi (după fiecare comandă, apăsați pe Enter):</span><span class="sxs-lookup"><span data-stu-id="7faaf-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="7faaf-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="7faaf-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="7faaf-120">După ce este generat fișierul text și apare pe ecran, salvați fișierul și atașați-l la solicitarea de serviciu.</span><span class="sxs-lookup"><span data-stu-id="7faaf-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
