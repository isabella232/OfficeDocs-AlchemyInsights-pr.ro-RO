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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="78188-102">Retragerea instrumentelor eDiscovery moștenite</span><span class="sxs-lookup"><span data-stu-id="78188-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="78188-103">Ca rezultat al funcționalităților eDiscovery noi și îmbunătățite din centrul de conformitate Microsoft 365, următoarele instrumente și commandlet de descoperire a informațiilor moștenite vor fi retrase în lunile următoare:</span><span class="sxs-lookup"><span data-stu-id="78188-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="78188-104">[Descoperirea informațiilor electronice](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) și [reținerea în locație](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) în centrul de administrare Exchange.</span><span class="sxs-lookup"><span data-stu-id="78188-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="78188-105">Cmdleturile PowerShell Exchange Online care acceptă descoperirea informațiilor electronice și rețineri în locație.</span><span class="sxs-lookup"><span data-stu-id="78188-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="78188-106">(Aceste cmdleturi sunt identificate în mod colectiv ca cmdleturi \*-MailboxSearch.) Aceasta include următoarele cmdleturi:</span><span class="sxs-lookup"><span data-stu-id="78188-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="78188-107">Nou-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="78188-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="78188-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="78188-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="78188-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="78188-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="78188-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="78188-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="78188-111">Cmdletul [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) din Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="78188-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="78188-112">Următoarele operațiuni în API-ul Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="78188-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="78188-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="78188-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="78188-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="78188-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="78188-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="78188-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="78188-116">Advanced eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="78188-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="78188-117">**Cronologie pentru retragere**:</span><span class="sxs-lookup"><span data-stu-id="78188-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="78188-118">**1 iulie 2020** Nu mai puteți crea noi căutări și rețineri, dar puteți să efectuați, să editați și să ștergeți căutările existente pe propriul risc.</span><span class="sxs-lookup"><span data-stu-id="78188-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="78188-119">Asistența Microsoft nu mai acceptă descoperirea în locație a informațiilor electronice & dețin în EAC.</span><span class="sxs-lookup"><span data-stu-id="78188-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="78188-120">**1 octombrie 2020** Descoperirea informațiilor electronice în locație & menține funcționalitatea în EAC va fi plasată în modul doar în citire, astfel încât să puteți elimina doar căutările și rezervările existente.</span><span class="sxs-lookup"><span data-stu-id="78188-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="78188-121">**Pentru mai multe informații, consultați**:</span><span class="sxs-lookup"><span data-stu-id="78188-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="78188-122">Migrarea căutărilor eDiscovery moștenite și reținerea la centrul de conformitate Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="78188-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="78188-123">Retragerea instrumentelor eDiscovery moștenite</span><span class="sxs-lookup"><span data-stu-id="78188-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="78188-124">Întrebări frecvente despre descoperirea informațiilor electronice și rețineri în locație</span><span class="sxs-lookup"><span data-stu-id="78188-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



