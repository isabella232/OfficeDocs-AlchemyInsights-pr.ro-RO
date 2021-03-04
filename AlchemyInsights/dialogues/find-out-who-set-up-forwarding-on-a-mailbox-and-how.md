---
title: Aflați cine a configurat redirecționarea la o cutie poștală și cum
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429992"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Aflați cine a configurat redirecționarea la o cutie poștală și cum

Dacă redirecționarea externă a fost setată la o cutie poștală, activitatea este auditată ca parte a cmdletului Set-Mailbox. Iată cum să găsiți activitatea în Jurnalul de auditare:

1. Accesați centrul de [conformitate & securitate Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Selectați căutare în >  **Jurnalul de auditare** căutare.
    > [!NOTE]
    > Dacă vedeți o notificare că trebuie să activați auditarea, mergeți mai departe și activați-o acum. Dacă această caracteristică nu este activată, rezultatele căutării nu vor putea să tragă date din datele anterioare.
1. Asigurați-vă că câmpul **activități** este setat să **afișeze rezultate pentru toate activitățile** (implicit). Specificați intervalul de date. Nu trebuie să specificați un nume de utilizator.
1. Selectați **Căutare**. Activitățile apar sub **Rezultate**.
1. Selectați **Filtrare rezultate**, apoi introduceți **Set-Mailbox** în câmpul Filtru **activitate** . Acest lucru returnează toate activitățile **Set-Mailbox** .
1. Pentru a vizualiza detaliile, selectați o activitate, apoi selectați **mai multe informații**. Sub **parametri** , puteți vedea adresa de e-mail de redirecționare setată în cutia poștală. **ID** -ul de utilizator reprezintă utilizatorul care a configurat redirecționarea externă în cutia poștală.
Pentru a afla mai multe, consultați [Căutați în Jurnalul de audit Office 365 pentru a depana scenarii comune](https://go.microsoft.com/fwlink/?linkid=2103944).