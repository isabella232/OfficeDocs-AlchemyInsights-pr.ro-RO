---
title: Depanarea redescoperirii ediscovery conține erori
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676280"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Depanarea redescoperirii ediscovery conține erori

Aveți probleme în legătură cu descoperirea informațiilor electronic? Iată câteva dintre cele mai bune practici de luat în considerare:

- Verificați starea distribuției în așteptare.  Dacă starea este **On (În așteptare) sau** **Dezactivat (În așteptare),** așteptați să se finalizeze distribuirea.
- Îmbinați actualizările pentru descoperirea informațiilor electronic într-o singură solicitare masivă, în loc să actualizați politica în mod repetat pentru fiecare tranzacție.
- Rulați Set-CaseHoldPolicy <policyname> -RetryDistribution în Powershell Centrul de securitate și conformitate. Pentru detalii, consultați [Consultați Conectare PowerShell pentru Centrul & securitate.](/powershell/exchange/connect-to-scc-powershell)

Pentru pașii necesari verificării acestor setări și a celor mai bune practici suplimentare pentru remedierea problemelor legate de descoperirea informațiilor electronic, consultați Depanarea erorilor de descoperire [a informațiilor electronic.](/microsoft-365/compliance/hold-distribution-errors)
Pentru informații despre depanarea altor probleme uzuale de descoperire a informațiilor electronic, consultați Investigarea, depanarea și [rezolvarea problemelor obișnuite de descoperire a informațiilor electronic.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
