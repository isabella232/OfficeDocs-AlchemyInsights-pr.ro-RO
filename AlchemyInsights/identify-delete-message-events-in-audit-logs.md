---
title: Identificarea evenimentelor de ștergere a mesajelor în jurnalele de auditare
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696525"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Jurnalele de audit pentru mesajele de e-mail șterse

Începând din ianuarie 2019, Microsoft pornește înregistrarea în jurnal a auditării cutiilor poștale în mod implicit. În caz contrar, pentru a revizui evenimentele de ștergere a mesajelor pentru un anumit utilizator, trebuie să activați manual acțiunile de ștergere pentru auditare. Dacă înregistrarea în jurnal a auditării cutiilor poștale este deja activată pentru organizația dumneavoastră sau pentru utilizatorul respectiv, urmați pașii de mai jos.

1. Conectați-vă la [Centrul de conformitate Microsoft 365 Security &](https://protection.office.com/)

2. Faceți clic pe **Căutare și investigație** și selectați **Căutare jurnal de auditare**.

3. Selectați intervalul de date din câmpurile data de **început** și **data de sfârșit** . Specificați numele de utilizator pentru utilizatorul pe care doriți să-l anchetați (utilizatorul care a șters elementele). În câmpul **activități** , selectați **mesaje șterse din folderul Elemente șterse** și **mutați mesajele în folderul Elemente șterse**.

4. Faceți clic pe **Căutare**.

În rezultate, selectați o înregistrare de audit. În flyout detalii, faceți clic pe **mai multe informații**. Informații suplimentare despre elementul șters (de exemplu, linia de subiect și locația elementului atunci când a fost șters) se afișează în câmpul **AffectedItems** . Proprietatea **ClientInfoString** va afișa dacă ștergerea a avut loc în Outlook, Outlook pe web (cunoscut anterior ca Outlook Web App) sau orice alt dispozitiv.

Pentru mai multe informații, consultați [cum se determină cine configurează redirecționarea e-mailului pentru o cutie poștală](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Notă**: nu puteți regăsi elemente șterse utilizând caracteristica jurnal de auditare. Pentru a regăsi mesajele șterse în Outlook pe web, consultați [Recuperarea elementelor șterse în Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
