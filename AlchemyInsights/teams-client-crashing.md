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
# <a name="teams-client-crashing"></a>Clientul Teams are căderi?

Dacă clientul dvs. Teams are căderi, încercați următoarele:

- Dacă utilizați aplicația desktop Teams, [asigurați-vă că aplicația este complet actualizată](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Asigurați-vă că toate adresele URL și intervalele de adrese [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) sunt accesibile.

- Conectați-vă cu contul de administrator al entității găzduite și verificați tabloul de bord [cu](https://docs.microsoft.com/office365/enterprise/view-service-health) starea serviciilor pentru a verifica dacă nu există nicio degradare sau degradare a serviciului.

- Dezinstalați și reinstalați aplicația Teams (link)
    - Navigați la folderul %appdata%\Microsoft\teams\ de pe computer și ștergeți toate fișierele din acel director.
    - [Descărcați și instalați aplicația Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), iar dacă este posibil, instalați Teams ca administrator (dați clic dreapta pe programul de instalare Teams și selectați "Rulați ca administrator", dacă este disponibil).

În cazul în care clientul dvs. Teams are în continuare probleme, puteți reproduce problema? Dacă da:

1. Utilizați înregistratorul de pași pentru a captura pașii.
    - Închideți TOATE aplicațiile inutile sau confidențiale.
    - Lansați înregistratorul de pași și reproduceți problema în timp ce sunteți conectat cu contul de utilizator afectat.
    - [Colectați jurnalele echipelor care capturează pașii de repro înregistrate.](https://docs.microsoft.com/microsoftteams/log-files) **Notă:** Asigurați-vă că capturați adresa de conectare a utilizatorului afectat.
    - Colectați e-mailul și/sau informațiile despre bucketul de eroare (Windows). Lansați windows Powershell pe computerul pe care are loc căderea și rulați următoarele comenzi:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Atașați fișierul la cazul dvs. de asistență.
