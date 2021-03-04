---
title: Erorile de sincronizare pentru înregistrare automată a dispozitivelor Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448934"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Erorile de sincronizare pentru înregistrare automată a dispozitivelor Apple

"Am detectat că aveți unul sau mai multe simboluri ADE/DEP care se află într-o stare de eroare. Până când starea erorii este rezolvată pentru fiecare simbol afectat, funcționalitatea ADE nu va funcționa așa cum vă așteptați. ".

Această eroare s-ar putea manifesta în mai multe moduri, inclusiv:

1. Este posibil ca dispozitivele să nu se sincronizeze de la ABM/ASM la Intune
2. Atribuirile de profil de înscriere pot fi nereușite
3. Este posibil ca dispozitivele să nu finalizeze cu succes înscrierea ADE

Verificați dacă eroarea de sincronizare a fost raportată în consola Intune de sub **dispozitive > Înscrieți dispozitivele > înscriere Apple > token**-ul programului de înscriere.

Una dintre cele mai comune cauze ale erorii de sincronizare este expirarea simbolului curent. În multe cazuri, reînnoirea simbolului afectat va rezolva problema.

Dacă una sau mai multe dintre jetoane a expirat, consultați următoarea documentație pentru a vă ajuta să le reînnoiți, după cum este necesar:

[Reînnoirea unui simbol de înscriere automată a dispozitivelor](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

În plus, puteți vedea următoarea documentație pentru a vedea potențialele remedieri pentru alte erori care cauzează erorile de sincronizare a tokenului:

[Erorile de sincronizare ABM/ASM pentru token-ul de înscriere a dispozitivelor automate pentru iOS/iPadOS și macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Erorile de sincronizare ABM/ASM pentru token-ul de înscriere a dispozitivelor automate pentru iOS/iPadOS și macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
