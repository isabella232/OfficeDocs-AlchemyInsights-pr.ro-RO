---
title: Probleme la conectarea la aplicațiile Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833016"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Remedierea aplicațiilor Microsoft 365 "Modulul Platformă de încredere al computerului nu funcționează corect"

Pentru a remedia această eroare, urmați pașii de mai jos:

- Instalați cele mai recente actualizări [pentru Windows](https://support.microsoft.com/help/4027667/windows-10-update) și [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Goliți acreditările Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) utilizând Managerul de acreditări Windows.<br/>
    **Notă:** Căile de registry pentru Office 2016 s-au modificat la 16.0. (De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)
- Încercați procesul [de recuperare a utilizatorului pentru](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) a remedia erorile Trusted Platform Module (TPM).
- Setați EnableADAL = 0 utilizând pașii următori:  
    1. Faceți clic dreapta pe butonul Start din Windows, **alegeți Rulare**, **tastați regedit**, apoi alegeți **OK.**
    2. Selectați **Da** pentru a permite editorului de registry să facă modificări la dispozitivul dvs.
    3. În Registry Editor, adăugați o valoare DWORD **de EnableADAL** cu o setare **0** sub HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Pentru mai multe informații, consultați Probleme de conectare la conectare după actualizarea la [Office 2016, compilarea 16.0.7967 din Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)