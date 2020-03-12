---
title: Retragerea instrumentelor eDiscovery moștenite
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600393"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Retragerea instrumentelor eDiscovery moștenite

Ca urmare a funcționalității eDiscovery noi și îmbunătățite în Centrul de conformitate Microsoft 365, următoarele instrumente și comenzi eDiscovery moștenite vor fi retrase în lunile următoare:

- [În-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) și [în loc deține](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) în centrul de administrare Exchange.

- Cmdlet-urile Exchange Online PowerShell care acceptă eDiscovery în loc și deține pe loc. (Aceste cmdlet-uri sunt identificate colectiv ca *-MailboxSearch cmdlet-uri.) Aceasta include următoarele cmdlet-uri:

    - [Căutare cutie poștală nouă](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Căutare cutie poștală de pornire](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Oprire-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch Set-MailboxCăutare](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdletul [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) în Exchange Online PowerShell.
- Următoarele operațiuni în API Exchange Web Services:
    - [GetSearchableCutii poștale](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnCutii poștale](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnCutii poștale](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Cronologie pentru pensionare:**
- 1 aprilie 2020: Nu veți putea crea căutări și rețineri noi, dar puteți să rulați, să editați și să ștergeți căutările existente pe propriul risc. Asistența Microsoft nu va mai accepta eDiscovery pe loc & deține în EAC.

- 1 iulie 2020: Funcționalitatea EDiscovery & Deține în EAC va fi plasată într-un mod doar în citire. Aceasta înseamnă că veți putea elimina căutările și reținerile existente.

**Pentru mai multe informații, consultați**:

 - [Migrarea căutărilor eDiscovery moștenite și deține la centrul de conformitate Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Retragerea instrumentelor eDiscovery moștenite](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Întrebări frecvente despre descoperirea electronică locală și deținerile pe loc](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



