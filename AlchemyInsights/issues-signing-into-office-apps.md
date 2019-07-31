---
title: Probleme de sign in la Office apps
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
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938312"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Fixarea Office apps "computerului Trusted Platformă module nu funcţionează corect" mesaj

Pentru a rezolva această eroare, încercaţi următoarele:

- Instalaţi cele mai recente actualizări pentru [Windows](https://support.microsoft.com/help/4027667/windows-10-update) si [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Acreditări clar Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Windows Credential Manager.<br/>
    **Notă:** Căi de registry pentru Office 2016 s-au schimbat la 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Încercaţi [procesul de recuperare utilizator](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) pentru a rezolva eşecurilor Trusted Platform Module (TPM).
- Set EnableADAL = 0 paşii următori:  
    1. Faceţi clic dreapta pe butonul Windows Start, selectaţi **Run**, tastaţi **regedit**şi apoi selectaţi **OK**.
    2. Selectați **Da** pentru a permite Registry Editor pentru a face modificări la aparatul dvs.
    3. În Registry Editor, adăugaţi o valoare DWORD **EnableADAL** cu o setare de **0** sub HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Pentru informaţii suplimentare, consultaţi [probleme de conexiune în semn-înăuntru după update la Office 2016 construi 16.0.7967 pe Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).