---
title: 'Eroare: regulile de pe acest computer nu se potrivește'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690975"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Eroare: regulile de pe acest computer nu se potrivește

Pentru a vedea starea actualizată a acestei probleme cunoscute, consultați [regulile de pe acest computer nu se potrivește cu regulile din Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Echipa Outlook a implementat o remediere în compilarea 12928,10000. Remedierea este deja la Insider rapid și va merge la Canalul lunar la sfârșitul lunii iunie 2020. După ce ați compilarea fixă, este posibil să primiți mesajul "ce reguli doriți să păstrați" pentru ultima dată. Alegeți server atunci când vi se solicită, apoi reveniți la Outlook și reactivați regulile care au fost dezactivate.

Până când remedierea este disponibilă, vă rugăm să utilizați următoarea soluție:

**Soluție**: în rapoartele recente, problema a avut loc pentru cele care au creat doar reguli client în Outlook desktop. Dacă continuați să întâmpinați problema, luați în considerare ștergerea regulilor, apoi creați și editați regulile doar în OWA (Outlook Web App) până când problema este rezolvată.

Dacă nu puteți șterge manual regulile, puteți executa o comandă Outlook atunci când porniți Outlook, rulând Outlook.exe/cleanrules. Acest lucru va șterge regulile client și server. Va șterge toate regulile pentru toate conturile din profilul Outlook. Această comandă este documentată în continuare în articolul parametri din linia de comandă.

