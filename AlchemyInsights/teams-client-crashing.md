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
# <a name="teams-client-crashing"></a>Teams client care se blochează

Dacă clientul dvs. Teams are căderi, încercați următoarele:

- Dacă utilizați aplicația desktop Teams, [asigurați-vă că aplicația este complet actualizată](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Asigurați-vă că [toate adresele URL Microsoft 365 adresele URL și intervalele de](/microsoftteams/connectivity-issues) adrese sunt accesibile.

- Conectați-vă cu contul de administrator al entității găzduite și verificați tabloul de bord [cu](/office365/enterprise/view-service-health) starea serviciilor pentru a verifica dacă nu există nicio degradare sau degradare a serviciului.

- Dezinstalarea și reinstalarea aplicației Teams Software
    - Navigați la folderul %appdata%\Microsoft\Teams\ de pe computer și ștergeți toate fișierele din acel director.
    - [Descărcați](https://www.microsoft.com/microsoft-teams/download-app)și instalați aplicația Teams și, dacă este posibil, instalați Teams ca administrator (faceți clic dreapta pe programul de instalare Teams și selectați Executare ca **administrator,** dacă este disponibil).

Dacă clientul Teams încă se blochează, încercați să reproduceți problema. Dacă puteți:

1. Utilizați înregistratorul de pași pentru a captura pașii.
    - Închideți TOATE aplicațiile inutile sau confidențiale.
    - Lansați înregistratorul de pași și reproduceți problema în timp ce sunteți conectat cu contul de utilizator afectat.
    - [Colectați jurnalele echipelor care capturează pașii de repro înregistrate.](/microsoftteams/log-files) **Notă:** Asigurați-vă că capturați adresa de conectare a utilizatorului afectat.
    - Colectați informațiile despre defecțiuni și/sau despre bucketul de eroare (Windows). Lansați Windows Powershell pe computerul pe care are loc căderea și rulați următoarele comenzi (după fiecare comandă, apăsați pe Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. După ce este generat fișierul text și apare pe ecran, salvați fișierul și atașați-l la solicitarea de serviciu. 
