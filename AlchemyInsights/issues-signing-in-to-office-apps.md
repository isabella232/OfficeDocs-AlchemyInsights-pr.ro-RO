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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833087"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Remedierea aplicațiilor Microsoft 365 Mesaj "Ne pare rău, un alt cont din organizația dvs. este deja conectat"

Pentru a remedia această eroare, urmați pașii de mai jos:

- Eliminați toate conturile de la locul de muncă, cu excepția contului afectat, utilizând Setări Windows > accesați contul de la locul **de muncă sau de la școală**.
- [Goliți acreditările Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Managerul de acreditări Windows.<br/>
    **Notă:** Căile de registry pentru Office 2016 s-au modificat la 16.0. (De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)
- Deschideți o aplicație Office, alegeți  >  **Deconectare**  >  **cont de fișier**. Apoi conectați-vă utilizând un cont de utilizator cu o licență validă. Pentru informații detaliate, consultați [Conturi din Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Pentru Mac, consultați [Nu vă puteți conecta la o aplicație Office 2016 pentru Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Pentru mai multe informații, consultați "Ne pare rău, un alt cont de la organizația [dvs. este deja conectat la acest computer" în Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)