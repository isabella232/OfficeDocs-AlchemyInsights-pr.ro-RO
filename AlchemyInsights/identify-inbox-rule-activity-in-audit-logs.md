---
title: Identificarea activității regulilor de inbox în jurnalele de auditare
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331135"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificarea activității regulilor de inbox în jurnalele de auditare

Puteți utiliza căutarea în jurnalul de auditare din Centru de conformitate Microsoft 365 pentru a vizualiza evenimentele regulilor de inbox (crearea, modificarea și ștergerea regulilor de inbox).

1. Urmați unul dintre pașii următori:
   - În programul Centru de conformitate Microsoft 365 la <https://compliance.microsoft.com> , accesați Audit  \> **soluții**. Sau, pentru a merge direct la **pagina Audit,** utilizați <https://compliance.microsoft.com/auditlogsearch> .
   - În portalul Microsoft 365 Defender din <https://security.microsoft.com> , accesați **Audit**. Sau, pentru a merge direct la **pagina Audit,** utilizați <https://security.microsoft.com/auditlogsearch> .

2. Pe fila **Căutare** din pagina **Audit,** configurați următoarele setări:
   - **Interval de timp și dată:** selectați intervalul de timp în **casetele Început** **și** Sfârșit.
   - **Activități:** Selectați una sau mai multe dintre următoarele valori:
     - **New-InboxRule Crearea regulii de inbox din Outlook Web App**
     - **Set-InboxRule Modificarea regulii din Outlook Web App**.
     - **Actualizarea regulilor pentru inbox Outlook client**

3. Când terminați, faceți clic pe **Căutare**. Activitățile apar pe noua pagină **Căutare audit.**

4. Selectați o activitate din rezultate pentru a deschide fereastra volant detalii. În câmpul Parametri se afișează informații despre setările **regulii** de inbox.

Pentru mai multe informații, [consultați Determinarea dacă un utilizator a creat o regulă de inbox.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
