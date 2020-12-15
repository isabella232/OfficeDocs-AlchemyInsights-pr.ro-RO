---
title: Instrument de diagnosticare a serviciului pentru desktopul virtual Windows
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680229"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Instrument de diagnosticare a serviciului pentru desktopul virtual Windows

Desktopul virtual Windows (WVD) oferă un instrument de diagnosticare care permite administratorilor să identifice erorile printr-o singură interfață. Acest instrument înregistrează informații legate de diagnosticare de fiecare dată când WVD este utilizat de o persoană atribuită un rol WVD. Fiecare jurnal conține informații despre rolul WVD implicat în activitate, mesajele de eroare care apar în timpul sesiunii și informațiile despre entitatea găzduită și utilizator. Analizele de jurnal Azure pot fi configurate pentru a captura Jurnalul de activități creat de instrumentul de diagnosticare. Iată cum se procedează:

1. Creați un spațiu de lucru de analiză jurnal cu [portalul Azure](https://go.microsoft.com/fwlink/?linkid=2129500) sau [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Conectați computerele Windows la Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Obțineți ID-ul spațiului de lucru și cheia principală a spațiului de lucru. Expertul de configurare are nevoie de aceste informații pentru a configura corect agentul și pentru a vă asigura că poate comunica cu Azure monitor.
1. [Împingeți datele de diagnosticare în spațiul de lucru](https://go.microsoft.com/fwlink/?linkid=2128284). Puteți să deconectați datele de diagnosticare de la entitatea găzduită WVD la analizele jurnal pentru spațiul de lucru.
1. [Identificați și diagnosticați problemele](https://go.microsoft.com/fwlink/?linkid=2128338) care sunt interne sau externe în legătură cu WVD.

Pentru a afla mai multe despre configurarea instrumentului de diagnosticare a serviciului pentru WVD, consultați [utilizarea analizei jurnal pentru caracteristica de diagnosticare](https://go.microsoft.com/fwlink/?linkid=2128084).
