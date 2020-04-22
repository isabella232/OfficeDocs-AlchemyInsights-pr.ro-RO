---
title: Pensionarea instrumentelor de descoperire electronică moștenită
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
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650580"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensionarea instrumentelor de descoperire electronică moștenită

Ca urmare a funcționalității eDiscovery noi și îmbunătățite în Centrul de conformitate Microsoft 365, următoarele instrumente și comenzi de descoperire electronică moștenite vor fi retrase în lunile următoare:

- [În locul eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) și [pe loc deține](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) în centrul de administrare Exchange.

- Cmdlet-urile Exchange Online PowerShell care acceptă local eDiscovery și In-Place deține. (Aceste cmdlet-uri sunt identificate colectiv ca cmdlet-uri *-MailboxSearch.) Aceasta include următoarele cmdlet-uri:

    - [Căutare a cutiilor poștale noi](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Pornire-Cutie poștalăCăutare](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Căutare a cutiei poștale](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Căutare a cutiilor poștale](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdletul [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) în Exchange Online PowerShell.
- Următoarele operațiuni în API Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnCutii de cutii poștale](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Cutii poștale GetHoldOn](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Avansate eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Calendarul pensionării:**
- 1 aprilie 2020: Nu veți putea crea căutări și deținenoi, dar puteți rula, edita și șterge căutările existente pe propriul risc. Microsoft Cină voință a voi nu lung cină In-Place eDiscovery & Deține în EAC.

- 1 iulie 2020: Funcționalitatea eDiscovery & Holds în EAC va fi plasată într-un mod doar în citire. Aceasta înseamnă că veți putea să eliminați căutările și deținerele existente numai.

**Pentru mai multe informații, consultați**:

 - [Migrarea căutărilor și dețineție de descoperire electronică moștenită la centrul de conformitate Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensionarea instrumentelor de descoperire electronică moștenită](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Întrebări frecvente despre descoperirea pe loc a imaginilor și dețineri pe loc](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



