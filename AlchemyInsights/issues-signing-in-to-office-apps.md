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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579949"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Remedierea microsoft 365 apps "Ne pare rău, un alt cont de la organizația dumneavoastră este deja conectat" mesaj

Pentru a remedia această eroare, urmați pașii de mai jos:

- Eliminați toate conturile de lucru, cu excepția contului afectat, utilizând Setări Windows > **la locul de muncă sau la școală**.
- [Goliți acreditările Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Windows Credential Manager.<br/>
    **Notã:** Căile de registry pentru Office 2016 s-au modificat la 16.0. (De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)
- Deschideți o aplicație Office, **alegeți**  >  **Account**  >  **Deconectare**cont de fișiere . Apoi conectați-vă utilizând un cont de utilizator cu o licență validă. Pentru informații detaliate, consultați [Conturi din Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Pentru Mac, consultați [Nu vă puteți conecta la o aplicație Office 2016 pentru Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Pentru mai multe informații, consultați ["Ne pare rău, un alt cont din organizația dvs.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)