---
title: Retragerea Instrumentelor de descoperire a informațiilor electronic moștenite
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
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798561"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Retragerea Instrumentelor de descoperire a informațiilor electronic moștenite

Ca urmare a funcționalității noi și îmbunătățite de descoperire a informațiilor electronic din Centrul de conformitate Microsoft 365, următoarele instrumente moștenite de descoperire a informațiilor electronic și a comenzilor vor fi retrase în lunile următoare:

- [Descoperirea informațiilor eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) și [in-place este](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) valabilă în centrul de administrare Exchange.

- Cmdleturi Exchange Online PowerShell care acceptă In-Place descoperirea informațiilor electronic și a In-Place reține. (Aceste cmdleturi sunt identificate colectiv drept cmdleturi *-MailboxSearch.) Între acestea, următoarele cmdleturi:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Căutarea set-mailbox](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Cmdletul Căutați](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) în cutia poștală din Exchange Online PowerShell.
- Următoarele operațiuni în API-ul Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Cronologie pentru pensionare:**
- **1 iulie 2020** Nu mai puteți să creați căutări noi și rețineri, dar puteți să rulați, să editați și să ștergeți căutări existente pe propriul risc. Asistența Microsoft nu mai acceptă In-Place reținerile în & eDiscovery în EAC.
    
- **1 octombrie 2020** In-Place eDiscovery & Păstrează funcționalitatea în EAC va fi plasată în modul doar în citire, astfel încât puteți elimina numai căutările existente și reținerile.

**Pentru mai multe informații, consultați:**

 - [Migrarea căutărilor de descoperire a informațiilor electronic moștenite și rețineri în Centrul de conformitate Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Retragerea instrumentelor moștenite de descoperire a informațiilor electronic](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Întrebări frecvente despre In-Place descoperirea informațiilor electronic și a In-Place rețineri](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



