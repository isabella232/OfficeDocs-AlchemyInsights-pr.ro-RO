---
title: Diminuarea erorii Aplicația nu a fost detectată
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810495"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Diminuarea erorii „Aplicația nu a fost detectată”

Eroarea de instalare a aplicației, „Aplicația nu a fost detectată după ce instalarea s-a finalizat cu succes”, raportată de Intune, poate apărea pe toate platformele de operare majore (Windows, iOS și Android).

Printre scenariile cele mai obișnuite care generează această eroare se numără:

- Aplicația a fost actualizată în afara Intune (de la un magazin de aplicații de la terți) după implementarea inițială. De exemplu, unele aplicații, cum ar fi Google Chrome, pot efectua actualizări automate.
- Un utilizator a dezinstalat aplicația după instalarea inițială.

Pentru a diminua această problemă, efectuați mai întâi o revizuire a dispozitivelor afectate pentru a determina scenariul în care apare eroarea.

- Dacă aplicația a fost actualizată în afara Intune, implementarea aplicației poate fi setată pentru a ignora versiunea aplicației. Pentru a face acest lucru, sub **Configurare aplicații > Informații despre aplicații**, setați **Ignorați versiunea aplicației** la **Da**.
- Atunci când țintește clientul, poate fi potrivit să implementați aplicația ca „obligatori” și să vă asigurați că este implementată cea mai recentă versiune.
- Ca alternativă, pe platforma iOS, puteți utiliza funcționalitatea **actualizare automată** asociată cu programul de achiziționare în volum Apple, care poate fi configurată să actualizeze automat la noile versiuni ale aplicației, pe măsură ce devin disponibile.

Pentru mai multe informații despre depanarea problemelor de instalare a aplicațiilor, consultați [Depanarea problemelor de instalare a aplicațiilor](https://docs.microsoft.com/intune/troubleshoot-app-install).
