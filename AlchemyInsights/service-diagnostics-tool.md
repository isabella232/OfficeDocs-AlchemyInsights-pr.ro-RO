---
title: Instrumentul de diagnosticare a serviciului pentru Desktop virtual Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595862"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Instrumentul de diagnosticare a serviciului pentru Desktop virtual Windows

Windows Virtual Desktop (WVD) oferă un instrument de diagnosticare care permite administratorilor să identifice erorile printr-o singură interfață. Acest instrument înregistrează informații legate de diagnosticare oricând WVD este utilizat de cineva cu un rol WVD. Fiecare jurnal conține informații despre rolul WVD implicat în activitate, mesajele de eroare care apar în timpul sesiunii și informațiile despre entitatea găzduită și utilizator. Azure Log Analytics poate fi configurat pentru a captura jurnalul de activitate creat de instrumentul de diagnosticare urmând acești pași:

1. Creați un spațiu de lucru Analiză jurnal cu [portalul Azure](https://go.microsoft.com/fwlink/?linkid=2129500) sau [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Conectați computerele Windows la Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913) Obțineți ID-ul spațiului de lucru și Cheia primară a spațiului de lucru. Expertul de instalare are nevoie de aceste informații pentru a configura corect agentul și a se asigura că poate comunica cu Azure Monitor.

1. [Împingeți date de diagnosticare în spațiul de lucru](https://go.microsoft.com/fwlink/?linkid=2128284). Puteți să împingeți date de diagnosticare din entitatea găzduită WVD în Analiza jurnalelor pentru spațiul de lucru.

1. [Identificați și diagnosticați](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemele interne sau externe legate de WVD.

Pentru a afla mai multe despre configurarea instrumentului de diagnosticare a serviciului pentru WVD, consultați Utilizarea analizelor de jurnal pentru caracteristica de diagnosticare.