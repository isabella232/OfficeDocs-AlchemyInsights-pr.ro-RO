---
title: Erori de sincronizare automată a înscrierii dispozitivelor Apple
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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013760"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Erori de sincronizare automată a înscrierii dispozitivelor Apple

"Am detectat că aveți unul sau mai multe simboluri ADE/DEP, care se află într-o stare de eroare. Până când se rezolvă starea de eroare pentru fiecare simbol afectat, funcționalitatea ADE nu va funcționa așa cum vă așteptați.".

Această eroare se poate manifesta în mai multe moduri, inclusiv:

1. Dispozitivele nu se pot sincroniza din ABM/ASM cu Intune
2. Este posibil ca atribuirile de profil de înscriere să nu reușesc
3. Este posibil ca dispozitivele să nu finalizeze cu succes înscrierea ADE

Căutați eroarea de sincronizare raportată în consola Intune sub Dispozitive **> Înscrieți dispozitivele > înscrierea Apple > simboluri pentru** programul de înscriere .

Una dintre cele mai comune cauze ale erorii de sincronizare este expirarea tokenului curent. În multe cazuri, reînnoirea tokenului afectat va rezolva problema.

Dacă unul sau mai multe simboluri au expirat, consultați documentația următoare pentru a vă ajuta să le reînnoiți după cum este necesar:

[Reînnoiți un token de înscriere automată a dispozitivului](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

În plus, puteți vedea documentația următoare pentru a vedea remedierile potențiale pentru alte erori care provoacă erori de sincronizare a simbolurilor:

[Erori de sincronizare ABM/ASM pentru simbolurile de înscriere automată a dispozitivelor pe iOS/iPadOS și macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Erori de sincronizare ABM/ASM pentru simbolurile de înscriere automată a dispozitivelor pe iOS/iPadOS și macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
