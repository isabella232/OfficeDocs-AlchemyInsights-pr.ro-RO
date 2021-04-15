---
title: 'Eroare: Regulile de pe acest computer nu se potrivesc'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782964"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="2c47d-102">Eroare: Regulile de pe acest computer nu se potrivesc</span><span class="sxs-lookup"><span data-stu-id="2c47d-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="2c47d-103">Pentru a vedea starea actualizată a acestei probleme cunoscute, consultați [Regulile de pe acest computer nu se potrivesc cu regulile din Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="2c47d-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="2c47d-104">Echipa Outlook a implementat o remediere în compilrea 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="2c47d-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="2c47d-105">Remedierea se află deja la Insider rapid și va ajunge pe Canalul lunar la sfârșitul lunii iunie 2020.</span><span class="sxs-lookup"><span data-stu-id="2c47d-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="2c47d-106">După ce obțineți compilrea fixă, este posibil să vi se solicite "Ce reguli doriți să păstrați" o ultimă dată.</span><span class="sxs-lookup"><span data-stu-id="2c47d-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="2c47d-107">Alegeți Server când vi se solicită, apoi reveniți în Outlook și reactivați toate regulile care au fost dezactivate.</span><span class="sxs-lookup"><span data-stu-id="2c47d-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="2c47d-108">Până când va fi disponibilă remedierea, utilizați următoarea soluție:</span><span class="sxs-lookup"><span data-stu-id="2c47d-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="2c47d-109">**Soluție: În** rapoartele recente, a apărut o problemă pentru cele care au creat doar reguli pentru clienți în Outlook pentru desktop.</span><span class="sxs-lookup"><span data-stu-id="2c47d-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="2c47d-110">Dacă problema continuă să se rezolve, luați în considerare ștergerea regulilor, apoi crearea și editarea regulilor doar în OWA (Outlook Web App) până când problema se rezolvă.</span><span class="sxs-lookup"><span data-stu-id="2c47d-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="2c47d-111">Dacă nu puteți șterge regulile manual, puteți rula o comandă Outlook atunci când porniți Outlook rulând Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="2c47d-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="2c47d-112">Acest lucru va șterge atât regulile client, cât și pe cele de server.</span><span class="sxs-lookup"><span data-stu-id="2c47d-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="2c47d-113">Se vor șterge toate regulile pentru toate conturile din Profilul Outlook.</span><span class="sxs-lookup"><span data-stu-id="2c47d-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="2c47d-114">Această comandă este documentată și în articolul Switch-uri în linia de comandă.</span><span class="sxs-lookup"><span data-stu-id="2c47d-114">This command is further documented in the Command-line switches article.</span></span>

