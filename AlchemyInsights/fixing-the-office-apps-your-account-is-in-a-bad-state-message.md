---
title: Remedierea aplicațiilor Microsoft 365 contul dumneavoastră este într-un mesaj de stare greșit
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744557"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Remedierea unei erori a aplicațiilor Microsoft 365 "contul dumneavoastră este într-o stare nepotrivită"

Pentru a remedia această eroare, încercați următoarele opțiuni pe computerul afectat:

- Deschideți o aplicație Office, selectați **File**  >  **Account**  >  **Deconectare cont fișier din toate conturile**. Conectați-vă din nou utilizând un cont de utilizator cu o licență validă. Pentru informații detaliate, consultați [Conturi din Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Debifați acreditările Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând managerul de acreditări Windows.<br>
  **Notă:** Căile de registry pentru Office 2016 s-au modificat la 16,0. De exemplu, \Software\Microsoft\Office\16.0\Common\Identity\
- Dacă eroarea apare în timp ce vă conectați la Office 365 utilizând Office 2013, [activați autentificarea modernă](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) pentru clientul Office.

Pentru mai multe informații, consultați [Depanarea aplicațiilor non-browser care nu se pot conecta la Microsoft 365, Azure sau Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

