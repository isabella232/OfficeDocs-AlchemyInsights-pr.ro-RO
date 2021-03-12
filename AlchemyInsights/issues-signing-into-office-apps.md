---
title: Probleme la conectarea la aplicațiile Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709118"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Remedierea aplicațiilor Microsoft 365 "modulul de platformă de încredere al computerului nu funcționează corect"

Pentru a remedia această eroare, urmați pașii de mai jos:

- Instalați cele mai recente actualizări pentru [Windows](https://support.microsoft.com/help/4027667/windows-10-update) și [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Debifați acreditările Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) utilizând managerul de acreditări Windows.<br/>
    **Notă:** Căile de registry pentru Office 2016 s-au modificat la 16,0. (De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)
- Încercați [procesul de recuperare a utilizatorilor](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) pentru a remedia eșecurile Trusted Platform Module (TPM).
- Setați EnableADAL = 0 utilizând următorii pași:  
    1. Faceți clic dreapta pe butonul Start din Windows, alegeți **rulare**, tastați **regedit**, apoi alegeți **OK**.
    2. Selectați **Da** pentru a permite Registry Editor să efectueze modificări pe dispozitivul dvs.
    3. În Registry Editor, adăugați o valoare DWORD **EnableADAL** cu o setare de **0** sub HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Pentru mai multe informații, consultați [probleme de conexiune în conectarea după actualizare la Office 2016 Build 16.0.7967 pe Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).