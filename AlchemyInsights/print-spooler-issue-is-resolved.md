---
title: Problema cu derulatorul de imprimare este rezolvată
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
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911350"
---
# <a name="print-spooler-issue-is-resolved"></a>Problema cu derulatorul de imprimare este rezolvată

Dacă dispozitivul dvs. a fost actualizat cu Windows 10 **19041.329** pentru sistem de operare, probabil că ați observat o problemă în care anumite imprimante nu se imprimă.   Derulatorul de imprimare poate să dea o eroare sau să se închidă în mod neașteptat atunci când încearcă să imprime și nu provine niciun rezultat de la imprimanta afectată. Această problemă este rezolvată în compilare sistem de operare  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Investigație continuă**

Fișierul LSASS (Local Security Authority Subsystem Service)**(Isass.exe)** poate să nu reușească pe unele dispozitive cu mesajul de eroare, "Un proces critic de sistem, C:\WINDOWS\system32\Isass.exe, nereușit cu codul de stare c0000008. Computerul trebuie repornit acum".  **Microsoft lucrează la o rezolvare și va furniza o actualizare într-o lansare viitoare.**

Pentru mai multe informații, consultați probleme [Windows 10 2004 cunoscute cu versiunea 2004.](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)