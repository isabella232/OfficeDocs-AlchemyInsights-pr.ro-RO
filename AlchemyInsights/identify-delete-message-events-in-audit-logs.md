---
title: Identificarea evenimentelor de mesaj de ștergere din jurnalele de auditare
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
ms.openlocfilehash: 7e13c9e5fbfa6ade065c2810150687085c1a9daae1a11c134688ec9a83ad37d9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54115660"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Jurnalele de auditare pentru mesajele de e-mail șterse

Începând din luna ianuarie 2019, Microsoft activarea implicită a înregistrării în jurnal pentru auditarea cutiilor poștale. În caz contrar, pentru a revizui evenimentele de mesaj de ștergere pentru un anumit utilizator, trebuie să activați manual acțiunile de ștergere pentru auditare. În cazul în care înregistrarea în jurnal de auditare pentru cutiile poștale este deja activată pentru organizația dvs. sau pentru utilizatorul specific, urmați pașii de mai jos.

1. Conectați-vă la [Centrul Microsoft 365 conformitate](https://protection.office.com/)

2. Faceți **clic pe Căutare și** investigare și **selectați Căutare în jurnalul de auditare.**

3. Selectați intervalul de date în **câmpurile Dată** de început **și Dată de** sfârșit. Specificați numele de utilizator pentru utilizatorul pe care doriți să-l investigați (utilizatorul care a șters elementele). În câmpul **Activități,** selectați Mesaje **șterse din folderul Elemente șterse și** **Mesaje mutate în folderul Elemente șterse.**

4. Faceți **clic pe Căutare.**

În rezultate, selectați o înregistrare de auditare. În fișa detalii, faceți clic **pe Mai multe informații**. Informații suplimentare despre elementul șters (de exemplu, linia de subiect și locația elementului atunci când a fost șters) se afișează în câmpul **Elemente afectate.** Proprietatea **ClientInfoString** se va afișa dacă ștergerea a avut loc în Outlook, Outlook pe web (cunoscut anterior ca Outlook Web App) sau pe orice alt dispozitiv.

Pentru mai multe informații, consultați [Determinarea cine a configurat redirecționarea e-mailului pentru o cutie poștală.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Notă:** Nu puteți regăsi elementele șterse utilizând caracteristica jurnal de auditare. Pentru a regăsi mesajele șterse în Outlook pe web, consultați [Recuperarea elementelor șterse din Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
