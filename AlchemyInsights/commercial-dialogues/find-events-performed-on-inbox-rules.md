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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313511"
---
# <a name="find-events-performed-on-inbox-rules"></a>Găsirea evenimentelor efectuate pentru reguli de inbox

Atunci când regulile de inbox sunt create, modificate sau șterse, evenimentele sunt înregistrate în jurnalul de auditare. Iată cum să le examinați:

1. Urmați una dintre următoarele acțiuni:
   - În programul Centru de conformitate Microsoft 365 la <https://compliance.microsoft.com> , accesați Audit  \> **soluții**. Sau, pentru a merge direct la **pagina Audit,** utilizați <https://compliance.microsoft.com/auditlogsearch> .
   - În portalul Microsoft 365 Defender din <https://security.microsoft.com> , accesați **Audit**. Sau, pentru a merge direct la **pagina Audit,** utilizați <https://security.microsoft.com/auditlogsearch> .

    **Notă:** dacă vedeți o notificare că trebuie să activați auditarea, activați-o acum. Dacă această caracteristică nu este activată, rezultatele căutării nu vor putea extrage date din datele anterioare.
1. Selectați câmpul Activități și găsiți Exchange cutie poștală, apoi selectați o New-InboxRule Creați o regulă de inbox din Outlook Web App. După ce terminați, faceți clic în afara panoului pentru a minimiza panoul Activități.
1. Specificați intervalul de date, apoi, în câmpul Utilizatori, selectați numele de utilizator al utilizatorului pe care doriți să-l investigați. Puteți selecta mai mulți utilizatori o dată.
1. Selectați Căutare. Activitățile apar sub Rezultate.
1. Pentru a vedea detaliile, selectați o activitate, apoi selectați Mai multe informații. Sub secțiunea Parametri puteți vedea numele regulii, setul de condiții și acțiunile pe care le va lua regula.

2. Pe fila **Căutare** din pagina **Audit,** configurați următoarele setări:
   - **Interval de timp și dată:** selectați intervalul de timp în **casetele Început** **și** Sfârșit.
   - **Activități:** **Selectați Nou-InboxRule Creați o regulă de inbox din Outlook Web App**

3. Când terminați, faceți clic pe **Căutare**. Activitățile apar pe noua pagină **Căutare audit.**

4. Selectați o activitate din rezultate pentru a deschide fereastra volant detalii. Sub **secțiunea Parametri** puteți vedea numele regulii, setul de condiții și acțiunile pe care le va lua regula.

Pentru a afla mai multe, consultați [Căutarea în jurnalul de auditare pentru a investiga problemele comune de asistență.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
