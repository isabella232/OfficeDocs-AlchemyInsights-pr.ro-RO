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
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981125"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Eroare: Regulile de pe acest computer nu se potrivesc

Pentru a vedea starea actualizată a acestei probleme cunoscute, consultați Regulile de pe acest computer nu se [potrivesc cu regulile din Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Echipa Outlook implementată o remediere în compilrea 12928.10000. Remedierea se află deja la Insider rapid și va ajunge pe Canalul lunar la sfârșitul lunii iunie 2020. După ce obțineți compilrea fixă, este posibil să vi se solicite "Ce reguli doriți să păstrați" o ultimă dată. Alegeți Server când vi se solicită, apoi reveniți în Outlook și reactivați toate regulile care au fost dezactivate.

Până când va fi disponibilă remedierea, utilizați următoarea soluție:

**Soluție: În** rapoartele recente, a apărut problema pentru cele care au creat doar reguli pentru clienți în Outlook desktop. Dacă problema se continuă, luați în considerare ștergerea regulilor, apoi crearea și editarea regulilor doar în OWA (Outlook Web App) până când problema se rezolvă.

Dacă nu puteți șterge regulile manual, puteți rula o comandă Outlook atunci când începeți Outlook rulând Outlook.exe /cleanrules. Acest lucru va șterge atât regulile client, cât și pe cele de server. Se vor șterge toate regulile pentru toate conturile din Outlook profil. Această comandă este documentată și în articolul Switch-uri în linia de comandă.

