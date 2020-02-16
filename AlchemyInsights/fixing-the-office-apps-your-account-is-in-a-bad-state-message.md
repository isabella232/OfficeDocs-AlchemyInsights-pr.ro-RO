---
title: Remedierea Aplicațiilor Office Contul dvs.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969715"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Remedierea aplicațiilor Office "Contul este într-o stare proastă" eroare

Pentru a remedia această eroare, încercați următoarele opțiuni pe computerul afectat:

- Deschideți o aplicație Office, selectați**Deconectare****cont** > de **fișiere** > din toate conturile . Conectați-vă din nou utilizând un cont de utilizator cu o licență validă. Pentru informații detaliate, consultați [Conturi în Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Goliți acreditările Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Managerul de acreditări Windows.<br>
  **Notã:** Căile de registry pentru Office 2016 s-au modificat la 16.0. De exemplu, \Software\Microsoft\Office\16.0\Common\Identity\
- Pe computerul afectat, setați EnableADAL = 0 utilizând următorii pași:  
     1. Faceți clic cu butonul din dreapta pe butonul Windows și selectați **Executare**. În caseta **Deschidere,** tastați **regedit**, apoi selectați **OK**.
     2. Selectați **Da** când vi se solicită să permiteți Editorului de registry să efectueze modificări pe dispozitiv.
    3. În Registry Editor, adăugați o valoare DWORD de EnableADAL cu o setare de 0 sub HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.
- Dacă apare eroarea în timp ce vă conectați la Office 365 utilizând Office 2013, [activați autentificarea modernă](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) pentru clientul Office.

Pentru mai multe informații, consultați [Cum se depanează aplicațiile non-browser care nu se pot conecta la Office 365, Azure sau Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

