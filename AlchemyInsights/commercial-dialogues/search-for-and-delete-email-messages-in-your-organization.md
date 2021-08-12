---
title: Căutarea și ștergerea mesajelor de e-mail din organizația dvs.
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948895"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Căutarea și ștergerea mesajelor de e-mail din organizația dvs.

Urmați acești pași:

1. Dacă nu sunt administrator global, pentru a căuta mesaje contul dvs. trebuie să fie adăugat la grupul de roluri **Manager pentru descoperirea** informațiilor electronic sau la rolul de gestionare a **căutării de conformitate.** Pentru a șterge mesaje, va trebui să vă asociați grupului **de roluri Gestionare organizație** sau rolului de gestionare a **căutării și ștergerii definitiv.** Permisiunile pentru aceste roluri sunt atribuite în Centrul de [conformitate & securitate.](https://protection.office.com)
2. [Creați o căutare de conținut](https://docs.microsoft.com/office365/securitycompliance/content-search) pentru a găsi mesajul de șters.
3. [Conectare la PowerShell din Centrul de & securitate și conformitate.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Dacă utilizați MFA, consultați aceste instrucțiuni: de la [Conectare Centrul de & PowerShell, utilizând Multi-Factor Authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Ștergeți mesajul: rulați `New-ComplianceSearchAction` cmdletul pentru a șterge mesajul. Mesajele șterse sunt mutate în folderul Elemente recuperabile al unui utilizator. Pentru o comandă de exemplu, [consultați Pasul 3: Ștergerea mesajului.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
