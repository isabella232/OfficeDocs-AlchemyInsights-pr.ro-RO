---
title: 'Eroare: Regulile de pe acest computer nu se potrivesc'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618025"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="5298d-102">Eroare: Regulile de pe acest computer nu se potrivesc</span><span class="sxs-lookup"><span data-stu-id="5298d-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="5298d-103">Pentru a vedea starea actualizată a acestei probleme cunoscute, consultați [Regulile de pe acest computer nu se potrivesc cu regulile din Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="5298d-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="5298d-104">Echipa Outlook a implementat o remediere în Build 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="5298d-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="5298d-105">Fix este deja la Insider Fast și va merge la Lunar Channel la sfârșitul lunii iunie 2020.</span><span class="sxs-lookup"><span data-stu-id="5298d-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="5298d-106">Odată ce ați fix construi s-ar putea obține prompt "Ce reguli vrei să păstreze" pentru ultima dată.</span><span class="sxs-lookup"><span data-stu-id="5298d-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="5298d-107">Alegeți Server atunci când vi se solicită și apoi reveniți în Outlook și reactivați orice reguli care au fost dezactivate.</span><span class="sxs-lookup"><span data-stu-id="5298d-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="5298d-108">Până când remedierea este disponibilă vă rugăm să utilizați următoarea soluție:</span><span class="sxs-lookup"><span data-stu-id="5298d-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="5298d-109">**Soluție**: În rapoartele recente, problema a apărut pentru cei care au creat numai reguli client în desktop Outlook.</span><span class="sxs-lookup"><span data-stu-id="5298d-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="5298d-110">Dacă continuați să executați problema, luați în considerare ștergerea regulilor și apoi creați și editați reguli numai în OWA (Outlook Web App) până când problema este rezolvată.</span><span class="sxs-lookup"><span data-stu-id="5298d-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="5298d-111">Dacă nu se poate șterge manual regulile, aveți posibilitatea să executați o comandă Outlook când porniți Outlook executând Reguli de curățare Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="5298d-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="5298d-112">Acest lucru va șterge atât regulile clientului, cât și ale serverului.</span><span class="sxs-lookup"><span data-stu-id="5298d-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="5298d-113">Acesta va șterge toate regulile pentru toate conturile din profilul Outlook.</span><span class="sxs-lookup"><span data-stu-id="5298d-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="5298d-114">Această comandă este documentată în continuare în articolul de comutare de linie de comandă.</span><span class="sxs-lookup"><span data-stu-id="5298d-114">This command is further documented in the Command-line switches  article.</span></span>