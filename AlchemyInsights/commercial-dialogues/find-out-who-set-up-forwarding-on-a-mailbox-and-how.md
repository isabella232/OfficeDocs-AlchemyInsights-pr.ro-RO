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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317820"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Aflați cine a configurat redirecționarea într-o cutie poștală și cum

Dacă redirecționarea externă a fost setată pentru o cutie poștală, activitatea este auditată ca parte a cmdletului **Set-Mailbox.** Iată cum să găsiți activitatea în jurnalul de auditare:

1. Urmați una dintre următoarele acțiuni:
   - În programul Centru de conformitate Microsoft 365 la <https://compliance.microsoft.com> , accesați Audit  \> **soluții**. Sau, pentru a merge direct la **pagina Audit,** utilizați <https://compliance.microsoft.com/auditlogsearch> .
   - În portalul Microsoft 365 Defender din <https://security.microsoft.com> , accesați **Audit**. Sau, pentru a merge direct la **pagina Audit,** utilizați <https://security.microsoft.com/auditlogsearch> .

   **Notă:** dacă vedeți o notificare că trebuie să activați auditarea, activați-o acum. Dacă această caracteristică nu este activată, rezultatele căutării nu vor putea extrage date din datele anterioare.

2. Pe pagina **Audit,** verificați dacă **este selectată** fila Căutare, apoi configurați următoarele setări:
   - Selectați intervalul de dată/oră în **casetele** **Început și** Sfârșit.
   - Caseta Verificare **activități** conține Afișare **rezultate pentru toate activitățile.**

3. Când terminați, faceți clic pe **Căutare**. Activitățile apar pe noua pagină **Căutare audit.**

4. În rezultate, faceți clic pe **coloana** Activitate pentru a sorta rezultatele și căutați **Intrări set-cutie poștală.**

5. Selectați o activitate din rezultate pentru a deschide fereastra volant detalii. Trebuie să priviți detaliile fiecărei înregistrări de auditare pentru a determina dacă activitatea este corelată cu redirecționarea e-mailului:
   - **ObjectId:** Valoarea alias a cutiei poștale care a fost modificată.
   - **Parametri:** _ForwardingSmtpAddress indică_ adresa de e-mail țintă.
   - **UserId:** Utilizatorul care a configurat redirecționarea e-mailului în cutia poștală **din câmpul ObjectId.**

Pentru mai multe informații, consultați [Determinarea cine a configurat redirecționarea e-mailului pentru o cutie poștală.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
