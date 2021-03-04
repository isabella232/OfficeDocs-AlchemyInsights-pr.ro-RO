---
title: Găsirea adresei IP în Jurnalul de auditare
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429788"
---
# <a name="find-the-ip-address-in-audit-log"></a>Găsirea adresei IP în Jurnalul de auditare

1. Adresa IP care corespunde unei activități efectuate de un utilizator sau administrator este afișată în jurnalele de auditare. Informațiile clientului sunt, de asemenea, înregistrate. Iată cum să identificați adresa IP:

1. Accesați centrul de [conformitate & securitate Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Selectați căutare în  >  **[Jurnalul de auditare](https://go.microsoft.com/fwlink/?linkid=2103759)** căutare.
    > [!NOTE]
    > Dacă vedeți o notificare că trebuie să activați auditarea, mergeți mai departe și activați-o acum. Dacă această caracteristică nu este activată, rezultatele căutării nu vor putea să tragă date din datele anterioare.
1. Dacă sunteți interesat de o anumită activitate, selectați-o din lista **activități** ; altfel, în mod implicit, toate activitățile vor fi returnate pentru utilizatorul selectat. Rețineți că este posibil ca anumite activități să nu fie disponibile pentru selecție din meniul **activități** ; cu toate acestea, acele elemente de audit vor fi returnate dacă se selectează **Afișare rezultate pentru toate activitățile** (setare implicită).
1. Specificați intervalul de date și, în câmpul **utilizatori** , selectați numele de utilizator al utilizatorului pe care doriți să-l anchetați.
1. Selectați **Căutare**. Activitățile apar sub **Rezultate**. Puteți vedea adresa IP pentru fiecare activitate.
1. Pentru a vizualiza detaliile, selectați o activitate, apoi selectați **mai multe informații**.

Pentru a afla mai multe, consultați căutați în [Jurnalul de audit Office 365 pentru a depana scenarii comune](https://go.microsoft.com/fwlink/?linkid=2103944).