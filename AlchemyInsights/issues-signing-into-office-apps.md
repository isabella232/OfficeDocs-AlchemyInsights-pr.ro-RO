---
title: Probleme la conectarea la aplicațiile Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579877"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Fixarea microsoft 365 apps "Modulul de încredere al computerului Platforma nu funcționează corect" mesaj

Pentru a remedia această eroare, urmați pașii de mai jos:

- Instalați cele mai recente actualizări pentru [Windows](https://support.microsoft.com/help/4027667/windows-10-update) și [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Goliți acreditările Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Windows Credential Manager.<br/>
    **Notã:** Căile de registry pentru Office 2016 s-au modificat la 16.0. (De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)
- Încercați procesul de [recuperare a utilizatorului](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) pentru a remedia erorile Trusted Platform Module (TPM).
- Setați EnableADAL = 0 utilizând următorii pași:  
    1. Faceți clic cu butonul din dreapta pe butonul Start din Windows, alegeți **Executare**, tastați **regedit**, apoi alegeți **OK**.
    2. Selectați **Da** pentru a permite Registry Editor să efectueze modificări pe dispozitiv.
    3. În Registry Editor, adăugați o valoare DWORD de **EnableADAL** cu o setare de **0** sub HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Pentru mai multe informații, consultați [Probleme de conexiune în conectare după actualizarea la Office 2016 build 16.0.7967 pe Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).