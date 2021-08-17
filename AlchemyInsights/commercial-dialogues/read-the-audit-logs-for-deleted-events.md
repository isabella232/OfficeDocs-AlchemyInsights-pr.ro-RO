---
title: Citirea jurnalelor de audit pentru evenimente șterse
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
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896027"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Citirea jurnalelor de audit pentru evenimente șterse

Iată cum să faceți acest lucru:

1. Urmați una dintre următoarele acțiuni:
   - În programul Centru de conformitate Microsoft 365 la <https://compliance.microsoft.com> , accesați Audit  \> **soluții**. Sau, pentru a merge direct la **pagina Audit,** utilizați <https://compliance.microsoft.com/auditlogsearch> .
   - În portalul Microsoft 365 Defender din <https://security.microsoft.com> , accesați **Audit**. Sau, pentru a merge direct la **pagina Audit,** utilizați <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Dacă vedeți o în prealabil că trebuie să activați caracteristica, activați-o acum. Dacă această caracteristică nu este activată, rezultatele căutării nu vor putea extrage date din datele anterioare.

2. Pe fila **Căutare** din pagina **Audit,** configurați următoarele setări:
   - **Interval de timp și dată:** selectați intervalul de timp în **casetele Început** **și** Sfârșit.
   - **Activități:** Introduceți Exchange **cutie poștală,** apoi selectați următoarele valori:
     - **S-au șters mesajele din folderul Elemente șterse**
     - **Mesajele au fost mutate în folderul Elemente șterse**

       După ce terminați, faceți clic în afara panoului pentru a minimiza **panoul** Activități.

   - **Utilizatori:** Acceptați valoarea implicită necompletată pentru a returna rezultate pentru toți utilizatorii sau introduceți unul sau mai mulți utilizatori.

3. Când terminați, faceți clic pe **Căutare**. Activitățile apar pe noua pagină **Căutare audit.**

4. Selectați o activitate din rezultate pentru a deschide fereastra volant detalii. Informațiile suplimentare despre elementul șters, cum ar fi linia de subiect și locația elementului atunci când acesta a fost șters, se afișează în câmpul **Elemente afectate.**

   > [!NOTE]
   > Nu puteți restaura elementele șterse utilizând caracteristica jurnal de auditare. Pentru a restaura elementele șterse, consultați [Recuperarea mesajelor de e-mail șterse din Outlook pe web](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Pentru mai multe informații, consultați Căutarea [în jurnalul de auditare pentru a investiga problemele comune de asistență.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
