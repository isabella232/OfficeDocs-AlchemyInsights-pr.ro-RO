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
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157684"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="27f9d-102">Retragerea instrumentelor eDiscovery moștenite</span><span class="sxs-lookup"><span data-stu-id="27f9d-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="27f9d-103">Ca urmare a funcționalității eDiscovery noi și îmbunătățite în Centrul de conformitate Microsoft 365, următoarele instrumente și comenzi eDiscovery moștenite vor fi retrase în lunile următoare:</span><span class="sxs-lookup"><span data-stu-id="27f9d-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="27f9d-104">[În-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) și [în loc deține](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) în centrul de administrare Exchange.</span><span class="sxs-lookup"><span data-stu-id="27f9d-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="27f9d-105">Cmdlet-urile Exchange Online PowerShell care acceptă eDiscovery în loc și deține pe loc.</span><span class="sxs-lookup"><span data-stu-id="27f9d-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="27f9d-106">(Aceste cmdlet-uri sunt identificate colectiv ca \*-MailboxSearch cmdlet-uri.) Aceasta include următoarele cmdlet-uri:</span><span class="sxs-lookup"><span data-stu-id="27f9d-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="27f9d-107">Căutare cutie poștală nouă</span><span class="sxs-lookup"><span data-stu-id="27f9d-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="27f9d-108">Căutare cutie poștală de pornire</span><span class="sxs-lookup"><span data-stu-id="27f9d-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="27f9d-109">Oprire-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="27f9d-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="27f9d-110">Set-MailboxSearch Set-MailboxCăutare</span><span class="sxs-lookup"><span data-stu-id="27f9d-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="27f9d-111">Cmdletul [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) în Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="27f9d-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="27f9d-112">Următoarele operațiuni în API Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="27f9d-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="27f9d-113">GetSearchableCutii poștale</span><span class="sxs-lookup"><span data-stu-id="27f9d-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="27f9d-114">SetHoldOnCutii poștale</span><span class="sxs-lookup"><span data-stu-id="27f9d-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="27f9d-115">GetHoldOnCutii poștale</span><span class="sxs-lookup"><span data-stu-id="27f9d-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="27f9d-116">Office 365 Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="27f9d-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="27f9d-117">**Cronologie pentru pensionare:**</span><span class="sxs-lookup"><span data-stu-id="27f9d-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="27f9d-118">1 aprilie 2020: Nu veți putea crea căutări și rețineri noi, dar puteți să rulați, să editați și să ștergeți căutările existente pe propriul risc.</span><span class="sxs-lookup"><span data-stu-id="27f9d-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="27f9d-119">Asistența Microsoft nu va mai accepta eDiscovery pe loc & deține în EAC.</span><span class="sxs-lookup"><span data-stu-id="27f9d-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="27f9d-120">1 iulie 2020: Funcționalitatea EDiscovery & Deține în EAC va fi plasată într-un mod doar în citire.</span><span class="sxs-lookup"><span data-stu-id="27f9d-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="27f9d-121">Aceasta înseamnă că veți putea elimina căutările și reținerile existente.</span><span class="sxs-lookup"><span data-stu-id="27f9d-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="27f9d-122">**Pentru mai multe informații, consultați**:</span><span class="sxs-lookup"><span data-stu-id="27f9d-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="27f9d-123">Migrarea căutărilor eDiscovery moștenite și deține la centrul de conformitate Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="27f9d-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="27f9d-124">Retragerea instrumentelor eDiscovery moștenite</span><span class="sxs-lookup"><span data-stu-id="27f9d-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="27f9d-125">Întrebări frecvente despre descoperirea electronică locală și deținerile pe loc</span><span class="sxs-lookup"><span data-stu-id="27f9d-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



