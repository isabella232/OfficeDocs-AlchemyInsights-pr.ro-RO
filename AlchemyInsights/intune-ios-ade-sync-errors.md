---
title: Erorile de sincronizare pentru înregistrare automată a dispozitivelor Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714978"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Erorile de sincronizare pentru înregistrare automată a dispozitivelor Apple

"Am detectat că aveți unul sau mai multe simboluri ADE/DEP care se află într-o stare de eroare. Până când starea erorii este rezolvată pentru fiecare simbol afectat, funcționalitatea ADE nu va funcționa la fel ".

Această eroare s-ar putea manifesta în mai multe moduri, inclusiv:

1. Este posibil ca dispozitivele să nu se sincronizeze de la ABM/ASM la Intune
2. Atribuirile de profil de înscriere pot fi nereușite
3. Este posibil ca dispozitivele să nu finalizeze cu succes înscrierea ADE

Verificați dacă eroarea de sincronizare a fost raportată în consola Intune de sub **dispozitive > Înscrieți dispozitivele > înscriere Apple > tokenuri de program de înscriere** și revizuiți următoarea documentație pentru a vedea orice remediere potențială:

[Erorile de sincronizare ABM/ASM pentru token-ul de înscriere a dispozitivelor automate pentru iOS/iPadOS și macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
