---
title: Identificarea evenimentelor de ștergere a mesajelor în jurnalele de auditare
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509000"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Jurnalele de audit pentru mesajele de e-mail șterse

Începând din ianuarie 2019, Microsoft pornește implicit înregistrarea în jurnal a auditului cutiei poștale. În caz contrar, pentru a examina ștergerea evenimentelor de mesaj pentru un anumit utilizator, trebuie să activați manual acțiunile de ștergere pentru auditare. Dacă înregistrarea în jurnal a auditului cutiei poștale este deja activată pentru organizația sau pentru utilizatorul specific, urmați pașii de mai jos.

1. Conectați-vă la Centrul de [conformitate Microsoft 365 Security &](https://protection.office.com/)

2. Faceți clic pe **Căutare și investigare** și selectați Căutare jurnal **audit**.

3. Selectați intervalul de date din câmpurile **Data de început** și data de **sfârșit.** Specificați numele de utilizator pentru utilizatorul pe care doriți să îl investigați (utilizatorul care a șters elementele). În câmpul **Activități,** selectați **Mesaje șterse din folderul Elemente șterse** și **Mesaje mutate în folderul Elemente șterse**.

4. Faceți clic pe **Căutare**.

În rezultate, selectați o înregistrare de audit. În detalii flyout, faceți clic pe **Mai multe informații**. Informații suplimentare despre elementul șters (de exemplu, linia de subiect și locația elementului când a fost șters) sunt afișate în câmpul **Elemente afectate.** Proprietatea **ClientInfoString** va afișa dacă ștergerea a avut loc în Outlook, Outlook pe web (cunoscut anterior ca Outlook Web App) sau orice alt dispozitiv.

Pentru mai multe informații, consultați [Determinarea cine a configurat redirecționarea e-mailului pentru o cutie poștală](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Notă:** Nu puteți regăsi elementele șterse utilizând caracteristica jurnal de auditare. Pentru a prelua mesajele șterse din Outlook pe web, consultați [Recuperarea elementelor șterse în Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
