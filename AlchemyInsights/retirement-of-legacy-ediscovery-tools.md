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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="dfca9-102">Retragerea Instrumentelor de descoperire a informațiilor electronic moștenite</span><span class="sxs-lookup"><span data-stu-id="dfca9-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="dfca9-103">Ca urmare a funcționalității noi și îmbunătățite de descoperire a informațiilor electronic din Centrul de conformitate Microsoft 365, următoarele instrumente moștenite de descoperire a informațiilor electronic și a comenzilor vor fi retrase în lunile următoare:</span><span class="sxs-lookup"><span data-stu-id="dfca9-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="dfca9-104">[Descoperirea informațiilor eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) și [in-place este](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) valabilă în centrul de administrare Exchange.</span><span class="sxs-lookup"><span data-stu-id="dfca9-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="dfca9-105">Cmdleturi Exchange Online PowerShell care acceptă In-Place descoperirea informațiilor electronic și a In-Place reține.</span><span class="sxs-lookup"><span data-stu-id="dfca9-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="dfca9-106">(Aceste cmdleturi sunt identificate colectiv drept cmdleturi \*-MailboxSearch.) Între acestea, următoarele cmdleturi:</span><span class="sxs-lookup"><span data-stu-id="dfca9-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="dfca9-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="dfca9-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="dfca9-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="dfca9-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="dfca9-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="dfca9-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="dfca9-110">Căutarea set-mailbox</span><span class="sxs-lookup"><span data-stu-id="dfca9-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="dfca9-111">[Cmdletul Căutați](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) în cutia poștală din Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="dfca9-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="dfca9-112">Următoarele operațiuni în API-ul Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="dfca9-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="dfca9-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="dfca9-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="dfca9-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="dfca9-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="dfca9-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="dfca9-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="dfca9-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="dfca9-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="dfca9-117">**Cronologie pentru pensionare:**</span><span class="sxs-lookup"><span data-stu-id="dfca9-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="dfca9-118">**1 iulie 2020** Nu mai puteți să creați căutări noi și rețineri, dar puteți să rulați, să editați și să ștergeți căutări existente pe propriul risc.</span><span class="sxs-lookup"><span data-stu-id="dfca9-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="dfca9-119">Asistența Microsoft nu mai acceptă In-Place reținerile în & eDiscovery în EAC.</span><span class="sxs-lookup"><span data-stu-id="dfca9-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="dfca9-120">**1 octombrie 2020** In-Place eDiscovery & Păstrează funcționalitatea în EAC va fi plasată în modul doar în citire, astfel încât puteți elimina numai căutările existente și reținerile.</span><span class="sxs-lookup"><span data-stu-id="dfca9-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="dfca9-121">**Pentru mai multe informații, consultați:**</span><span class="sxs-lookup"><span data-stu-id="dfca9-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="dfca9-122">Migrarea căutărilor de descoperire a informațiilor electronic moștenite și rețineri în Centrul de conformitate Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="dfca9-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="dfca9-123">Retragerea instrumentelor moștenite de descoperire a informațiilor electronic</span><span class="sxs-lookup"><span data-stu-id="dfca9-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="dfca9-124">Întrebări frecvente despre In-Place descoperirea informațiilor electronic și a In-Place rețineri</span><span class="sxs-lookup"><span data-stu-id="dfca9-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



