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
ms.openlocfilehash: 258e92368b8a33e8ea807f0cb9af90132c86ed5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58303589"
---
# <a name="find-the-ip-address-in-audit-log"></a>Găsirea adresei IP în jurnalul de auditare

Adresa IP care corespunde unei activități efectuate de un utilizator sau un administrator este afișată în jurnalele de auditare. De asemenea, informațiile despre client sunt înregistrate în jurnal. Iată cum să identificați adresa IP:

1. Urmați una dintre următoarele acțiuni:
   - În programul Centru de conformitate Microsoft 365 la <https://compliance.microsoft.com> , accesați Audit  \> **soluții**. Sau, pentru a merge direct la **pagina Audit,** utilizați <https://compliance.microsoft.com/auditlogsearch> .
   - În portalul Microsoft 365 Defender din <https://security.microsoft.com> , accesați **Audit**. Sau, pentru a merge direct la **pagina Audit,** utilizați <https://security.microsoft.com/auditlogsearch> .

    **Notă:** dacă vedeți o notificare că trebuie să activați auditarea, activați-o acum. Dacă această caracteristică nu este activată, rezultatele căutării nu vor putea extrage date din datele anterioare.

2. Pe pagina **Audit,** verificați dacă **este selectată** fila Căutare, apoi configurați următoarele setări:
   - **Interval de timp și dată:** selectați intervalul de timp în **casetele Început** **și** Sfârșit.
   - **Activități:** Dacă vă interesează o anumită activitate, selectați-o din listă; în caz contrar, valoarea implicită **Afișați rezultate pentru toate activitățile** returnează toate activitățile. Rețineți că este posibil ca anumite activități să nu fie disponibile pentru selecție; totuși, elementele de auditare respective vor fi returnate **dacă s-a selectat Afișare rezultate** pentru toate activitățile.
   - **Utilizatori:** Acceptați valoarea implicită necompletată pentru a returna rezultate pentru toți utilizatorii sau introduceți unul sau mai mulți utilizatori.

3. Când terminați, faceți clic pe **Căutare**. Activitățile apar pe noua pagină **Căutare audit.**

4. În rezultate, faceți clic **pe Filtrare rezultate** și tastați **Set-Mailbox** în caseta de filtrare de activitate.

5. Selectați o înregistrare de auditare din rezultate pentru a **deschide fereastra** volanată Detalii.

Pentru mai multe informații, consultați Căutarea [în jurnalul de auditare pentru a investiga problemele comune de asistență.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
