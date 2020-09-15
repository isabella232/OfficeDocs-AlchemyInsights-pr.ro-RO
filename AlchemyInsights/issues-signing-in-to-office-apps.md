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
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695335"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Remedierea aplicațiilor Microsoft 365 "Ne pare rău, un alt cont din organizație este deja conectat" mesaj

Pentru a remedia această eroare, urmați pașii de mai jos:

- Eliminați toate conturile de lucru, cu excepția contului afectat, utilizând setările Windows > **Access la locul de muncă sau la școală**.
- [Debifați acreditările Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând managerul de acreditări Windows.<br/>
    **Notă:** Căile de registry pentru Office 2016 s-au modificat la 16,0. (De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)
- Deschideți o aplicație Office, alegeți **File**  >  **Account**  >  **Deconectare**cont fișier. Apoi conectați-vă utilizând un cont de utilizator cu o licență validă. Pentru informații detaliate, consultați [Conturi din Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Pentru Mac, consultați [Nu vă puteți conecta la o aplicație Office 2016 pentru Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Pentru mai multe informații, consultați ["Ne pare rău, un alt cont din organizație este deja conectat la acest computer" în Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).