---
title: Găsirea evenimentelor efectuate pentru reguli de inbox
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
ms.openlocfilehash: 14a5a18bc1422572db567c9533fefe5a7e0120afd64df4a64623038cc063ce93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058662"
---
# <a name="find-events-performed-on-inbox-rules"></a>Găsirea evenimentelor efectuate pentru reguli de inbox

Atunci când regulile de inbox sunt create, modificate sau șterse, evenimentele sunt înregistrate în jurnalul de auditare. Iată cum să le examinați:

1. Accesați Centrul de [Office 365 securitate & conformitate](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Selectați Căutare > căutare în jurnalul de auditare.

    > [!NOTE]
    > Dacă vedeți o notificare că trebuie să activați auditarea, activați-o acum. Dacă această caracteristică nu este activată, rezultatele căutării nu vor putea extrage date din datele anterioare.
1. Selectați câmpul Activități și găsiți activitățile Exchange cutie poștală, apoi New-InboxRule Creați o regulă de inbox din Outlook Web App. După ce terminați, faceți clic în afara panoului pentru a minimiza panoul Activități.
1. Specificați intervalul de date, apoi, în câmpul Utilizatori, selectați numele de utilizator al utilizatorului pe care doriți să-l investigați. Puteți selecta mai mulți utilizatori o dată.
1. Selectați Căutare. Activitățile apar sub Rezultate.
1. Pentru a vedea detaliile, selectați o activitate, apoi selectați Mai multe informații. Sub secțiunea Parametri puteți vedea numele regulii, setul de condiții și acțiunile pe care le va lua regula.

Pentru a afla mai multe, consultați Căutarea în Office 365 de auditare pentru a depana scenarii comune.