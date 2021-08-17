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
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890350"
---
# <a name="teams-client-crashing"></a>Teams client care se blochează

Dacă clientul dvs. Teams are căderi, încercați următoarele:

- Dacă utilizați aplicația desktop Teams, [asigurați-vă că aplicația este complet actualizată](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Asigurați-vă că [toate adresele URL Microsoft 365 adresele URL și intervalele de](https://docs.microsoft.com/microsoftteams/connectivity-issues) adrese sunt accesibile.

- Conectați-vă cu contul de administrator al entității găzduite și verificați tabloul de bord [cu](https://docs.microsoft.com/office365/enterprise/view-service-health) starea serviciilor pentru a verifica dacă nu există nicio degradare sau degradare a serviciului.

- Dezinstalarea și reinstalarea aplicației Teams Software
    - Navigați la folderul %appdata%\Microsoft\Teams\ de pe computer și ștergeți toate fișierele din acel director.
    - [Descărcați](https://www.microsoft.com/microsoft-teams/download-app)și instalați aplicația Teams și, dacă este posibil, instalați Teams ca administrator (faceți clic dreapta pe programul de instalare Teams și selectați Executare ca **administrator,** dacă este disponibil).

Dacă clientul Teams încă se blochează, încercați să reproduceți problema. Dacă puteți:

1. Utilizați înregistratorul de pași pentru a captura pașii.
    - Închideți TOATE aplicațiile inutile sau confidențiale.
    - Lansați înregistratorul de pași și reproduceți problema în timp ce sunteți conectat cu contul de utilizator afectat.
    - [Colectați jurnalele echipelor care capturează pașii de repro înregistrate.](https://docs.microsoft.com/microsoftteams/log-files) **Notă:** Asigurați-vă că capturați adresa de conectare a utilizatorului afectat.
    - Colectați de e-mailul și/sau informațiile despre bucketul de eroare (Windows). Lansați Windows Powershell pe computerul pe care are loc căderea și rulați următoarele comenzi (după fiecare comandă, apăsați pe Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. După ce este generat fișierul text și apare pe ecran, salvați fișierul și atașați-l la solicitarea de serviciu. 
