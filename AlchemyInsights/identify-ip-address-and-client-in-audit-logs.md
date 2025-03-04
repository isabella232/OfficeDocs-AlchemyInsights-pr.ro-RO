---
title: Identificarea adresei IP și a clientului în jurnalele de auditare
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 57a1756787f8297a2a1ab3012b95aaa2f33e6045
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313031"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificarea adresei IP și a clientului în jurnalele de auditare

Adresa IP care corespunde unei activități a unui utilizator sau administrator Microsoft 365 este afișată în Jurnalele de auditare. De asemenea, informațiile despre client sunt înregistrate în jurnal. Iată pașii pentru identificarea acestor informații

1. Conectați-vă la [Centrul Microsoft 365 conformitate](https://protection.office.com/).

2. Accesați pagina Căutare **în jurnalul**  >  **de auditare.**

   Dacă vă interesează o anumită activitate, selectați-o din **lista** Activități. Dacă nu, toate activitățile vor fi returnate pentru utilizatorul selectat (setare implicită).

   **Notă:** este posibil ca anumite activități să nu fie disponibile **în meniul** Activități; totuși, elementele de auditare respective vor fi returnate **dacă s-a selectat Afișare** rezultate pentru toate activitățile (setare implicită).

3. Specificați numele de utilizator în **câmpul Utilizatori,** selectați intervalul de date corespunzător pentru activitate, apoi faceți clic pe **Căutare.**

În rezultate, puteți vedea adresa IP pentru acea activitate în panoul de rezultate. Selectați înregistrarea de audit pentru a vedea informații detaliate în fișa **Detalii** (de exemplu, Client, Utilizator care a efectuat acțiunea etc.).

Pentru mai multe informații, [consultați Găsirea adresei IP a computerului utilizat pentru a accesa un cont compromis.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
