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
# <a name="teams-client-crashing"></a>Clientul Teams are căderi?

Dacă clientul dvs. Teams are căderi, încercați următoarele:

- Dacă utilizați aplicația desktop Teams, [asigurați-vă că aplicația este complet actualizată](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Asigurați-vă că toate [adresele URL Microsoft 365 și intervalele de adrese](https://docs.microsoft.com/microsoftteams/connectivity-issues) sunt accesibile.

- Conectați-vă cu contul de administrator al entității găzduite și verificați [Tabloul de bord de sănătate serviciu](https://docs.microsoft.com/office365/enterprise/view-service-health) pentru a verifica dacă nu există nicio întrerupere sau degradare a serviciului.

- Dezinstalarea și reinstalarea aplicației Teams (link)
    - Navigați la folderul %appdata%\Microsoft\teams\ de pe computer și ștergeți toate fișierele din acel director.
    - [Descărcați și instalați aplicația Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)și, dacă este posibil, instalați Teams ca administrator (faceți clic dreapta pe programul de instalare Teams și selectați "Executare ca administrator", dacă este disponibil).

Dacă clientul tău Teams încă se prăbușește, poți reproduce problema? Dacă da:

1. Utilizați Înregistratorul de pași pentru a captura pașii.
    - Închideți toate aplicațiile inutile sau confidențiale.
    - Lansați Înregistratorul de pași și reproduceți problema în timp ce faceți Log in cu contul de utilizator afectat.
    - [Colecta jurnalele de echipe care captează pașii de repro înregistrate](https://docs.microsoft.com/microsoftteams/log-files). **Notă:** Asigurați-vă că capturați adresa de conectare a utilizatorului afectat.
    - Colectați informațiile despre dump și/sau din găleata de defecte (Windows). Lansarea Windows Powershell pe computerul în cazul în care se produce accident și executați următoarele comenzi:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Atașați fișierul la cazul de asistență.
