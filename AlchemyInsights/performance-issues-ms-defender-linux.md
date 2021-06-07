---
title: Probleme de performanță pentru Microsoft Defender pentru punct final în Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794000"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Probleme de performanță pentru Microsoft Defender pentru punct final în Linux

Acest articol vă îndrumă prin pașii de identificare a problemelor de performanță pentru Microsoft Defender pentru punct final pe Linux.

Este important să verificați mai întâi dacă problema cu care vă confruntați se rezolvă cu cea mai [recentă versiune](/microsoft-365/security/defender-endpoint/linux-whatsnew). 

Pentru a începe investigarea, consultați [Depanarea problemelor de performanță pentru Microsoft Defender pentru punct final pe Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Excluderi

Excluderile pot contribui la atenuarea problemelor de performanță. Revizuiți excluderile înainte de a începe, astfel încât orice risc suplimentar să fie cunoscut și documentat.

Pentru mai multe informații, consultați [Configurarea și validarea excluderilor pentru Microsoft Defender pentru punctul final pe Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Atunci când aveți mai multe fișiere & foldere de exclus și toate se rezidă în același loc, ar putea fi mai ușor să excludeți muntele. Începând cu lansarea din februarie 101.22.80, puteți exclude un punct de munte întreg.

De exemplu, dacă /mnt/backup este un punct de munte, puteți adăuga /mnt/backup la lista de excluderi rulezând această comandă:

`$ mdatp exclusion folder add –path /mnt/backup`

**Notă:** Adăugarea excluderilor mărește riscul de detectare a malware-ului și ar trebui gestionat și implementat cu grijă.

## <a name="need-help"></a>Aveți nevoie de ajutor?

Pentru a vă asista în modul cel mai eficient, colectați datele de diagnosticare înainte de a deschide un caz de asistență.
