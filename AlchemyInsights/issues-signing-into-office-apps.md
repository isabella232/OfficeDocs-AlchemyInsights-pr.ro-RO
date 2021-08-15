---
title: Probleme la conectarea la Microsoft 365 uri
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
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986903"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Remedierea Microsoft 365 mesaje "Modulul platformă de încredere al computerului nu funcționează corect"

Pentru a remedia această eroare, urmați pașii de mai jos:

- Instalați cele mai recente actualizări [pentru Windows](https://support.microsoft.com/help/4027667/windows-10-update) și [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Goliți Office acreditările](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) utilizând Windows de acreditări.<br/>
    **Notă:** Căile de registry pentru Office 2016 s-au modificat la 16.0. (De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)
- Încercați procesul [de recuperare a utilizatorului pentru](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) a remedia erorile Trusted Platform Module (TPM).
- Setați EnableADAL = 0 utilizând pașii următori:  
    1. Faceți clic dreapta pe Windows Start, **alegeți Rulare**, tastați **regedit**, apoi alegeți **OK**.
    2. Selectați **Da** pentru a permite editorului de registry să facă modificări la dispozitivul dvs.
    3. În Registry Editor, adăugați o valoare DWORD **de EnableADAL** cu o setare **0** sub HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Pentru mai multe informații, consultați Probleme de conectare după actualizarea la [Office 2016 compilarea 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)pe Windows 10 .