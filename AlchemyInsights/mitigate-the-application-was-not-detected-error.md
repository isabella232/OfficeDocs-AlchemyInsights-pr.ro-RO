---
title: Diminuarea erorii Aplicația nu a fost detectată
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666990"
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
