---
title: 'Eroare: regulile de pe acest computer nu se potrivește'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690975"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="89d85-102">Eroare: regulile de pe acest computer nu se potrivește</span><span class="sxs-lookup"><span data-stu-id="89d85-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="89d85-103">Pentru a vedea starea actualizată a acestei probleme cunoscute, consultați [regulile de pe acest computer nu se potrivește cu regulile din Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="89d85-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="89d85-104">Echipa Outlook a implementat o remediere în compilarea 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="89d85-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="89d85-105">Remedierea este deja la Insider rapid și va merge la Canalul lunar la sfârșitul lunii iunie 2020.</span><span class="sxs-lookup"><span data-stu-id="89d85-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="89d85-106">După ce ați compilarea fixă, este posibil să primiți mesajul "ce reguli doriți să păstrați" pentru ultima dată.</span><span class="sxs-lookup"><span data-stu-id="89d85-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="89d85-107">Alegeți server atunci când vi se solicită, apoi reveniți la Outlook și reactivați regulile care au fost dezactivate.</span><span class="sxs-lookup"><span data-stu-id="89d85-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="89d85-108">Până când remedierea este disponibilă, vă rugăm să utilizați următoarea soluție:</span><span class="sxs-lookup"><span data-stu-id="89d85-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="89d85-109">**Soluție**: în rapoartele recente, problema a avut loc pentru cele care au creat doar reguli client în Outlook desktop.</span><span class="sxs-lookup"><span data-stu-id="89d85-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="89d85-110">Dacă continuați să întâmpinați problema, luați în considerare ștergerea regulilor, apoi creați și editați regulile doar în OWA (Outlook Web App) până când problema este rezolvată.</span><span class="sxs-lookup"><span data-stu-id="89d85-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="89d85-111">Dacă nu puteți șterge manual regulile, puteți executa o comandă Outlook atunci când porniți Outlook, rulând Outlook.exe/cleanrules.</span><span class="sxs-lookup"><span data-stu-id="89d85-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="89d85-112">Acest lucru va șterge regulile client și server.</span><span class="sxs-lookup"><span data-stu-id="89d85-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="89d85-113">Va șterge toate regulile pentru toate conturile din profilul Outlook.</span><span class="sxs-lookup"><span data-stu-id="89d85-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="89d85-114">Această comandă este documentată în continuare în articolul parametri din linia de comandă.</span><span class="sxs-lookup"><span data-stu-id="89d85-114">This command is further documented in the Command-line switches article.</span></span>

