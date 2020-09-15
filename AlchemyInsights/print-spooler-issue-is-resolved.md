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
# <a name="print-spooler-issue-is-resolved"></a>Problema de derulare a imprimării este rezolvată

Dacă dispozitivul a fost actualizat cu Windows 10  **OS Build 19041,329**, este posibil să fi observat o problemă în care anumite imprimante nu reușesc să se imprime. Derulator de imprimare poate să arunce o eroare sau să se închidă în mod neașteptat atunci când încercați să imprimați și nicio ieșire nu provine de la imprimanta afectată. Această problemă este rezolvată în sistemul de operare generare  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Investigație în curs**

Fișierul local Security Authority (LSASS) (**Isass.exe**) este posibil să nu reușească pe unele dispozitive cu mesajul de eroare "un proces de sistem critic, C:\WINDOWS\system32\Isass.exe, nu a reușit cu codul de stare c0000008. Mașina trebuie repornită acum ".  **Microsoft lucrează la o rezoluție și va furniza o actualizare într-o lansare viitoare.**

Pentru mai multe informații, consultați  [probleme cunoscute cu Windows 10 Version 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).