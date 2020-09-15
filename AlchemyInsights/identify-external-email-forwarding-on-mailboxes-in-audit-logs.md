---
title: Identificarea redirecționarii e-mailurilor externe în cutiile poștale din jurnalele de audit
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696309"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificarea când se configurează redirecționarea e-mailurilor externe în cutiile poștale

Atunci când un utilizator Microsoft 365 configurează redirecționarea e-mailurilor externe într-o cutie poștală, activitatea este auditată ca parte din cmdletul **Set-Mailbox** . Puteți vedea activitatea utilizând căutarea în Jurnalul de audit din centrul de conformitate & de securitate.

1. Conectați-vă la [Centrul de conformitate Microsoft 365 Security &](https://protection.office.com/).

2. Accesați **Search**  >  pagina**Căutare în Jurnalul de auditare** căutare.

3. Selectați intervalul de date din câmpurile data de **început** și **data de sfârșit** . Nu trebuie să specificați un nume de utilizator. Verificați dacă câmpul **activități** este setat să **afișeze rezultate pentru toate activitățile**.

4. Faceți clic pe **Căutare**.

În rezultate, faceți clic pe **Filtrare rezultate** și tastați **set-cutie poștală** în caseta Filtru activitate. Selectați o înregistrare de auditare în rezultate. În flyout **Detalii** , faceți clic pe **mai multe informații**. Trebuie să examinați detaliile fiecărei înregistrări de audit pentru a determina dacă activitatea este corelată cu redirecționarea e-mailului.

- **ObjectID**: valoarea alias a cutiei poștale care a fost modificată.

- **Parametri**: _ForwardingSmtpAddress_ indică adresa de e-mail țintă.

- **ID**utilizator: utilizatorul care a configurat redirecționarea mesajelor de e-mail în cutia poștală din câmpul **objectID** .

Pentru mai multe informații, consultați [cum se determină cine configurează redirecționarea e-mailului pentru o cutie poștală](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
