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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="053fc-102">Pensionarea instrumentelor de descoperire electronică moștenită</span><span class="sxs-lookup"><span data-stu-id="053fc-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="053fc-103">Ca urmare a funcționalității eDiscovery noi și îmbunătățite în Centrul de conformitate Microsoft 365, următoarele instrumente și comenzi de descoperire electronică moștenite vor fi retrase în lunile următoare:</span><span class="sxs-lookup"><span data-stu-id="053fc-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="053fc-104">[În locul eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) și [pe loc deține](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) în centrul de administrare Exchange.</span><span class="sxs-lookup"><span data-stu-id="053fc-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="053fc-105">Cmdlet-urile Exchange Online PowerShell care acceptă local eDiscovery și In-Place deține.</span><span class="sxs-lookup"><span data-stu-id="053fc-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="053fc-106">(Aceste cmdlet-uri sunt identificate colectiv ca cmdlet-uri \*-MailboxSearch.) Aceasta include următoarele cmdlet-uri:</span><span class="sxs-lookup"><span data-stu-id="053fc-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="053fc-107">Căutare a cutiilor poștale noi</span><span class="sxs-lookup"><span data-stu-id="053fc-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="053fc-108">Pornire-Cutie poștalăCăutare</span><span class="sxs-lookup"><span data-stu-id="053fc-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="053fc-109">Căutare a cutiei poștale</span><span class="sxs-lookup"><span data-stu-id="053fc-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="053fc-110">Căutare a cutiilor poștale</span><span class="sxs-lookup"><span data-stu-id="053fc-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="053fc-111">Cmdletul [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) în Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="053fc-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="053fc-112">Următoarele operațiuni în API Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="053fc-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="053fc-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="053fc-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="053fc-114">SetHoldOnCutii de cutii poștale</span><span class="sxs-lookup"><span data-stu-id="053fc-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="053fc-115">Cutii poștale GetHoldOn</span><span class="sxs-lookup"><span data-stu-id="053fc-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="053fc-116">Avansate eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="053fc-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="053fc-117">**Calendarul pensionării:**</span><span class="sxs-lookup"><span data-stu-id="053fc-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="053fc-118">1 aprilie 2020: Nu veți putea crea căutări și deținenoi, dar puteți rula, edita și șterge căutările existente pe propriul risc.</span><span class="sxs-lookup"><span data-stu-id="053fc-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="053fc-119">Microsoft Cină voință a voi nu lung cină In-Place eDiscovery & Deține în EAC.</span><span class="sxs-lookup"><span data-stu-id="053fc-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="053fc-120">1 iulie 2020: Funcționalitatea eDiscovery & Holds în EAC va fi plasată într-un mod doar în citire.</span><span class="sxs-lookup"><span data-stu-id="053fc-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="053fc-121">Aceasta înseamnă că veți putea să eliminați căutările și deținerele existente numai.</span><span class="sxs-lookup"><span data-stu-id="053fc-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="053fc-122">**Pentru mai multe informații, consultați**:</span><span class="sxs-lookup"><span data-stu-id="053fc-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="053fc-123">Migrarea căutărilor și dețineție de descoperire electronică moștenită la centrul de conformitate Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="053fc-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="053fc-124">Pensionarea instrumentelor de descoperire electronică moștenită</span><span class="sxs-lookup"><span data-stu-id="053fc-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="053fc-125">Întrebări frecvente despre descoperirea pe loc a imaginilor și dețineri pe loc</span><span class="sxs-lookup"><span data-stu-id="053fc-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



