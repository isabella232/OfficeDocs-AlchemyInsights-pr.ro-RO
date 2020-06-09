---
title: 'Eroare: Regulile de pe acest computer nu se potrivesc'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618025"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Eroare: Regulile de pe acest computer nu se potrivesc

Pentru a vedea starea actualizată a acestei probleme cunoscute, consultați [Regulile de pe acest computer nu se potrivesc cu regulile din Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Echipa Outlook a implementat o remediere în Build 12928.10000. Fix este deja la Insider Fast și va merge la Lunar Channel la sfârșitul lunii iunie 2020. Odată ce ați fix construi s-ar putea obține prompt "Ce reguli vrei să păstreze" pentru ultima dată. Alegeți Server atunci când vi se solicită și apoi reveniți în Outlook și reactivați orice reguli care au fost dezactivate.

Până când remedierea este disponibilă vă rugăm să utilizați următoarea soluție:

**Soluție**: În rapoartele recente, problema a apărut pentru cei care au creat numai reguli client în desktop Outlook. Dacă continuați să executați problema, luați în considerare ștergerea regulilor și apoi creați și editați reguli numai în OWA (Outlook Web App) până când problema este rezolvată.

Dacă nu se poate șterge manual regulile, aveți posibilitatea să executați o comandă Outlook când porniți Outlook executând Reguli de curățare Outlook.exe /cleanrules. Acest lucru va șterge atât regulile clientului, cât și ale serverului. Acesta va șterge toate regulile pentru toate conturile din profilul Outlook. Această comandă este documentată în continuare în articolul de comutare de linie de comandă.