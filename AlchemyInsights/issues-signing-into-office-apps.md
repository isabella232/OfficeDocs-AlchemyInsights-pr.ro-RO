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
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695191"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Remedierea aplicațiilor Microsoft 365 "modulul de platformă de încredere al computerului nu funcționează corect"

Pentru a remedia această eroare, urmați pașii de mai jos:

- Instalați cele mai recente actualizări pentru [Windows](https://support.microsoft.com/help/4027667/windows-10-update) și [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Debifați acreditările Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând managerul de acreditări Windows.<br/>
    **Notă:** Căile de registry pentru Office 2016 s-au modificat la 16,0. (De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)
- Încercați [procesul de recuperare a utilizatorilor](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) pentru a remedia eșecurile Trusted Platform Module (TPM).
- Setați EnableADAL = 0 utilizând următorii pași:  
    1. Faceți clic dreapta pe butonul Start din Windows, alegeți **rulare**, tastați **regedit**, apoi alegeți **OK**.
    2. Selectați **Da** pentru a permite Registry Editor să efectueze modificări pe dispozitivul dvs.
    3. În Registry Editor, adăugați o valoare DWORD **EnableADAL** cu o setare de **0** sub HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Pentru mai multe informații, consultați [probleme de conexiune în conectarea după actualizare la Office 2016 Build 16.0.7967 pe Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).