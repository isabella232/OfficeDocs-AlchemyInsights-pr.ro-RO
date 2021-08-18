---
title: Identificarea redirecționării externe a e-mailurilor în cutiile poștale din jurnalele de auditare
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331171"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificarea atunci când este configurată redirecționarea e-mailului extern pentru cutiile poștale

Atunci când Microsoft 365 utilizator configurează redirecționarea externă a e-mailurilor pentru o cutie poștală, activitatea este auditată ca parte a cmdletului **Set-Mailbox.** Puteți vedea activitatea utilizând căutarea în jurnalul de auditare. Iată cum să faceți acest lucru.

1. Urmați unul dintre pașii următori:
   - În programul Centru de conformitate Microsoft 365 la <https://compliance.microsoft.com> , accesați Audit  \> **soluții**. Sau, pentru a merge direct la **pagina Audit,** utilizați <https://compliance.microsoft.com/auditlogsearch> .
   - În portalul Microsoft 365 Defender din <https://security.microsoft.com> , accesați **Audit**. Sau, pentru a merge direct la **pagina Audit,** utilizați <https://sip.security.microsoft.com/auditlogsearch> .

2. Pe pagina **Audit,** verificați dacă **este selectată** fila Căutare, apoi configurați următoarele setări:
   - Selectați intervalul de dată/oră în **casetele** **Început și** Sfârșit.
   - Caseta Verificare **activități** conține Afișare **rezultate pentru toate activitățile.**

3. Când terminați, faceți clic pe **Căutare**. Activitățile apar pe noua pagină **Căutare audit.**

4. În rezultate, faceți clic **pe Filtrare rezultate** și tastați **Set-Mailbox** în caseta de filtrare de activitate.

5. Selectați o înregistrare de auditare în rezultate. În **fișa Detalii,** faceți clic **pe Mai multe informații**. Trebuie să priviți detaliile fiecărei înregistrări de auditare pentru a determina dacă activitatea este corelată cu redirecționarea e-mailului.

   - **ObjectId:** Valoarea alias a cutiei poștale care a fost modificată.
   - **Parametri:** _ForwardingSmtpAddress indică_ adresa de e-mail țintă.
   - **UserId:** Utilizatorul care a configurat redirecționarea e-mailului în cutia poștală **din câmpul ObjectId.**

Pentru mai multe informații, consultați [Determinarea cine a configurat redirecționarea e-mailului pentru o cutie poștală.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
