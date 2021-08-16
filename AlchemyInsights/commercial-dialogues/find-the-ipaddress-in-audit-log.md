---
title: Găsirea adresei IP în jurnalul de auditare
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 5b58803719df700290f495cb2d2d6742f072420a2a1d393534ca165bb5a14fbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017144"
---
# <a name="find-the-ip-address-in-audit-log"></a>Găsirea adresei IP în jurnalul de auditare

1. Adresa IP care corespunde unei activități efectuate de un utilizator sau un administrator este afișată în jurnalele de auditare. De asemenea, informațiile despre client sunt înregistrate în jurnal. Iată cum să identificați adresa IP:

1. Accesați Centrul de [Office 365 securitate & conformitate](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Selectați **Căutare**  >  **[în jurnalul de auditare.](https://go.microsoft.com/fwlink/?linkid=2103759)**
    > [!NOTE]
    > Dacă vedeți o notificare că trebuie să activați auditarea, activați-o acum. Dacă această caracteristică nu este activată, rezultatele căutării nu vor putea extrage date din datele anterioare.
1. Dacă vă interesează o anumită activitate, selectați-o din **lista** Activități; altfel, în mod implicit, toate activitățile vor fi returnate pentru utilizatorul selectat. Rețineți că este posibil ca anumite activități să nu fie disponibile pentru selectare **din meniul** Activități; totuși, elementele de auditare respective vor fi returnate **dacă s-a selectat Afișare** rezultate pentru toate activitățile (setare implicită).
1. Specificați intervalul de date și, în câmpul Utilizatori, **selectați** numele de utilizator al utilizatorului pe care doriți să-l investigați.
1. Selectați **Căutare**. Activitățile apar sub **Rezultate**. Puteți vedea adresa IP pentru fiecare activitate.
1. Pentru a vedea detaliile, selectați o activitate, apoi selectați **Mai multe informații.**

Pentru mai multe informații, consultați Căutarea în [jurnalul Office 365 auditare pentru a depana scenarii comune.](https://go.microsoft.com/fwlink/?linkid=2103944)