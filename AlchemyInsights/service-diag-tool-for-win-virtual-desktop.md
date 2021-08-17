---
title: Service diagnostics tool for Windows Virtual Desktop
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052398"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Service diagnostics tool for Windows Virtual Desktop

Windows Desktop virtual (WVD) oferă un instrument de diagnosticare care permite administratorilor să identifice erorile printr-o singură interfață. Acest instrument înregistrează informații legate de diagnosticare oricând WVD este utilizat de cineva cu un rol WVD. Fiecare jurnal conține informații despre rolul WVD implicat în activitate, mesajele de eroare care apar în timpul sesiunii și informațiile despre entitatea găzduită și utilizator. Azure Log Analytics poate fi configurat pentru a captura jurnalul de activitate creat de instrumentul de diagnosticare. Iată cum se procedează:

1. Creați un spațiu de lucru Analiză jurnal cu [portalul Azure](https://go.microsoft.com/fwlink/?linkid=2129500) sau [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Conectare Windows computere pe Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913) Obțineți ID-ul spațiului de lucru și Cheia primară a spațiului de lucru. Expertul de instalare are nevoie de aceste informații pentru a configura corect agentul și a se asigura că poate comunica cu Azure Monitor.
1. [Împingeți date de diagnosticare în spațiul de lucru](https://go.microsoft.com/fwlink/?linkid=2128284). Puteți să împingeți date de diagnosticare din entitatea găzduită WVD în Analiza jurnalelor pentru spațiul de lucru.
1. [Identificați și diagnosticați problemele](https://go.microsoft.com/fwlink/?linkid=2128338) interne sau externe legate de WVD.

Pentru a afla mai multe despre configurarea instrumentului de diagnosticare a serviciului pentru WVD, consultați Utilizarea [analizei jurnalului pentru caracteristica de diagnosticare.](https://go.microsoft.com/fwlink/?linkid=2128084)
