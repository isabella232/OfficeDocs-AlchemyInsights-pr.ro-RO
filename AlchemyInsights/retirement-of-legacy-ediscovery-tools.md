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
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074686"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Retragerea Instrumentelor de descoperire a informațiilor electronic moștenite

Ca urmare Microsoft 365 noii și îmbunătățite funcționalități eDiscovery din Centrul de conformitate Microsoft 365, următoarele instrumente de descoperire a informațiilor electronic și a comenzilor moștenite vor fi retrase în lunile următoare:

- [Descoperirea informațiilor electronic local și](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) în [reținere în](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) cadrul centrului Exchange administrare.

- The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds. (Aceste cmdleturi sunt identificate colectiv drept cmdleturi *-MailboxSearch.) Între acestea, următoarele cmdleturi:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Căutarea set-mailbox](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Cmdletul Căutați](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) în cutia poștală Exchange Online PowerShell.
- Următoarele operațiuni cu api-Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Cronologie pentru pensionare:**
- **1 iulie 2020** Nu mai puteți să creați căutări noi și rețineri, dar puteți să rulați, să editați și să ștergeți căutări existente pe propriul risc. Asistența Microsoft nu mai acceptă In-Place reținerile în & eDiscovery în EAC.
    
- **1 octombrie 2020** In-Place eDiscovery & Păstrează funcționalitatea în EAC va fi plasată în modul doar în citire, astfel încât puteți elimina numai căutările existente și reținerile.

**Pentru mai multe informații, consultați:**

 - [Migrarea căutărilor de descoperire a informațiilor electronic moștenite și migrează în Centru de conformitate Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Retragerea instrumentelor moștenite de descoperire a informațiilor electronic](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Întrebări frecvente despre In-Place descoperirea informațiilor electronic și a In-Place rețineri](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



