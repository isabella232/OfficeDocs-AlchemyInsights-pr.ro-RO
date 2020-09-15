---
title: Problema de derulare a imprimării este rezolvată
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801853"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="efad5-102">Problema de derulare a imprimării este rezolvată</span><span class="sxs-lookup"><span data-stu-id="efad5-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="efad5-103">Dacă dispozitivul a fost actualizat cu Windows 10  **OS Build 19041,329**, este posibil să fi observat o problemă în care anumite imprimante nu reușesc să se imprime.</span><span class="sxs-lookup"><span data-stu-id="efad5-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="efad5-104">Derulator de imprimare poate să arunce o eroare sau să se închidă în mod neașteptat atunci când încercați să imprimați și nicio ieșire nu provine de la imprimanta afectată.</span><span class="sxs-lookup"><span data-stu-id="efad5-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="efad5-105">Această problemă este rezolvată în sistemul de operare generare  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="efad5-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="efad5-106">**Investigație în curs**</span><span class="sxs-lookup"><span data-stu-id="efad5-106">**Ongoing investigation**</span></span>

<span data-ttu-id="efad5-107">Fișierul local Security Authority (LSASS) (**Isass.exe**) este posibil să nu reușească pe unele dispozitive cu mesajul de eroare "un proces de sistem critic, C:\WINDOWS\system32\Isass.exe, nu a reușit cu codul de stare c0000008.</span><span class="sxs-lookup"><span data-stu-id="efad5-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="efad5-108">Mașina trebuie repornită acum ".</span><span class="sxs-lookup"><span data-stu-id="efad5-108">The machine must now be restarted".</span></span>  <span data-ttu-id="efad5-109">**Microsoft lucrează la o rezoluție și va furniza o actualizare într-o lansare viitoare.**</span><span class="sxs-lookup"><span data-stu-id="efad5-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="efad5-110">Pentru mai multe informații, consultați  [probleme cunoscute cu Windows 10 Version 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="efad5-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>