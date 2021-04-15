---
title: 'Eroare: Regulile de pe acest computer nu se potrivesc'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782964"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Eroare: Regulile de pe acest computer nu se potrivesc

Pentru a vedea starea actualizată a acestei probleme cunoscute, consultați [Regulile de pe acest computer nu se potrivesc cu regulile din Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Echipa Outlook a implementat o remediere în compilrea 12928.10000. Remedierea se află deja la Insider rapid și va ajunge pe Canalul lunar la sfârșitul lunii iunie 2020. După ce obțineți compilrea fixă, este posibil să vi se solicite "Ce reguli doriți să păstrați" o ultimă dată. Alegeți Server când vi se solicită, apoi reveniți în Outlook și reactivați toate regulile care au fost dezactivate.

Până când va fi disponibilă remedierea, utilizați următoarea soluție:

**Soluție: În** rapoartele recente, a apărut o problemă pentru cele care au creat doar reguli pentru clienți în Outlook pentru desktop. Dacă problema continuă să se rezolve, luați în considerare ștergerea regulilor, apoi crearea și editarea regulilor doar în OWA (Outlook Web App) până când problema se rezolvă.

Dacă nu puteți șterge regulile manual, puteți rula o comandă Outlook atunci când porniți Outlook rulând Outlook.exe /cleanrules. Acest lucru va șterge atât regulile client, cât și pe cele de server. Se vor șterge toate regulile pentru toate conturile din Profilul Outlook. Această comandă este documentată și în articolul Switch-uri în linia de comandă.

