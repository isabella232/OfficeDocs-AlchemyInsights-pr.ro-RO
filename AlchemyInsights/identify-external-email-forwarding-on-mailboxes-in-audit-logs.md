---
title: Identifica externe e-mail forwarding pe cutiile poştale în jurnalele de auditare
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417223"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifica atunci când extern e-mail forwarding este configurat pe cutiile poştale

Atunci când un utilizator se configurează externe e-mail forwarding pe o cutie poştală, activitatea este auditate ca parte a cmdlet-ul **Set-Mailbox** . Puteţi vedea activitatea folosind audit jurnal caută în & de securitate centru de conformitate.

1. Conectaţi-vă la [Centrul de conformitatea Office 365 securitate &](https://protection.office.com/)

2. Faceţi clic pe **Căutare şi ancheta** şi selectaţi **Căutare de jurnalul de Audit**.

3. Selectaţi intervalul de date în câmpurile **data de început** şi **data de sfârşit** . Nu aveţi nevoie să specificaţi un nume de utilizator. Verificaţi câmpul de **activităţi** este setată pentru a **afişa rezultate pentru toate acțiunile**.

4. Faceţi clic pe **Căutare**.

În rezultate, faceţi clic pe **Filtru rezultate** şi **Set-Mailbox** de tip în caseta filtru de activitate. Selectaţi o înregistrare de audit în rezultate. În fișă de **Detalii** , faceţi clic pe **mai multe informaţii**. Trebuie sa te uiti la detalii cu privire la fiecare înregistrare de audit pentru a determina dacă activitatea este legată de e-mail forwarding.

- **ObjectId**: valoarea aliasul cutiei poştale care s-a modificat.

- **Parametrii**: _ForwardingSmtpAddress_ indică adresa de email ţintă.

- **ID utilizator**: utilizatorului care a configurat expediere poştă electronică din cutia poştală în domeniul **ObjectId** .

Pentru informaţii suplimentare, consultaţi [determină care configurarea e-mail forwarding pentru o cutie poştală](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
