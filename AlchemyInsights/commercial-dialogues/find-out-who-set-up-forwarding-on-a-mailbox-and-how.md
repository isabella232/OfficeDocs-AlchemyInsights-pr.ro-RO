---
title: Aflați cine a configurat redirecționarea într-o cutie poștală și cum
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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988219"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Aflați cine a configurat redirecționarea într-o cutie poștală și cum

Dacă redirecționarea externă a fost setată pentru o cutie poștală, activitatea este auditată ca parte Set-Mailbox cmdletului nou. Iată cum să găsiți activitatea în jurnalul de auditare:

1. Accesați Centrul de [Office 365 securitate & conformitate](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Selectați **Căutare** >  **în jurnalul de auditare.**
    > [!NOTE]
    > Dacă vedeți o notificare că trebuie să activați auditarea, activați-o acum. Dacă această caracteristică nu este activată, rezultatele căutării nu vor putea extrage date din datele anterioare.
1. Asigurați-vă **că în** câmpul Activități este setat să se **afișează rezultate pentru toate activitățile** (setarea implicită). Specificați intervalul de date. Nu trebuie să specificați un nume de utilizator.
1. Selectați **Căutare**. Activitățile apar sub **Rezultate**.
1. Selectați **Filtrare** rezultate , apoi introduceți **Set-mailbox** în **câmpul de** filtrare Activitate. Returnează toate **activitățile Set-Mailbox.**
1. Pentru a vedea detaliile, selectați o activitate, apoi selectați Mai **multe informații.** Sub **Parametri puteți vedea** adresa de e-mail de redirecționare care a fost setată în cutia poștală. **ID-ul** de utilizator reprezintă utilizatorul care a configurat redirecționarea externă pentru cutia poștală.
Pentru mai multe informații, consultați [Căutarea în jurnalul Office 365 auditare pentru a depana scenarii comune.](https://go.microsoft.com/fwlink/?linkid=2103944)