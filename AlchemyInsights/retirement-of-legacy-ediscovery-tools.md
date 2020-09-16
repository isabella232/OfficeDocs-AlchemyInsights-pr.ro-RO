---
title: Retragerea instrumentelor eDiscovery moștenite
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
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727795"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Retragerea instrumentelor eDiscovery moștenite

Ca rezultat al funcționalităților eDiscovery noi și îmbunătățite din centrul de conformitate Microsoft 365, următoarele instrumente și commandlet de descoperire a informațiilor moștenite vor fi retrase în lunile următoare:

- [Descoperirea informațiilor electronice](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) și [reținerea în locație](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) în centrul de administrare Exchange.

- Cmdleturile PowerShell Exchange Online care acceptă descoperirea informațiilor electronice și rețineri în locație. (Aceste cmdleturi sunt identificate în mod colectiv ca cmdleturi *-MailboxSearch.) Aceasta include următoarele cmdleturi:

    - [Nou-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdletul [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) din Exchange Online PowerShell.
- Următoarele operațiuni în API-ul Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Cronologie pentru retragere**:
- **1 iulie 2020** Nu mai puteți crea noi căutări și rețineri, dar puteți să efectuați, să editați și să ștergeți căutările existente pe propriul risc. Asistența Microsoft nu mai acceptă descoperirea în locație a informațiilor electronice & dețin în EAC.
    
- **1 octombrie 2020** Descoperirea informațiilor electronice în locație & menține funcționalitatea în EAC va fi plasată în modul doar în citire, astfel încât să puteți elimina doar căutările și rezervările existente.

**Pentru mai multe informații, consultați**:

 - [Migrarea căutărilor eDiscovery moștenite și reținerea la centrul de conformitate Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Retragerea instrumentelor eDiscovery moștenite](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Întrebări frecvente despre descoperirea informațiilor electronice și rețineri în locație](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



