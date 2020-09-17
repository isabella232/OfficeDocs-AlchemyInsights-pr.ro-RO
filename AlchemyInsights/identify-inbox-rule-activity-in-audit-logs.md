---
title: Identificarea activității de regulă Inbox în jurnalele de auditare
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
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779063"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificarea activității de regulă Inbox în jurnalele de auditare

Puteți utiliza căutarea în Jurnalul de audit din centrul de conformitate Microsoft 365 Security & pentru a vizualiza evenimentele de regulă pentru Inbox (crearea, modificarea și ștergerea regulilor pentru Inbox).

1. Conectați-vă la [Centrul de conformitate Microsoft 365 Security &](https://protection.office.com/).

2. Accesați **Search**  >  pagina**Căutare în Jurnalul de auditare** căutare.

3. Selectați intervalul de date din câmpurile data de **început** și **data de sfârșit** .

4. Sub **activități de cutie poștală Exchange**, Verificați dacă câmpul **activități** este setat la **nou-InboxRule creare/modificare/Activare/Dezactivare regulă Inbox**.

5. Faceți clic pe **Căutare**.

În rezultate, selectați o înregistrare de audit. În flyout detalii, faceți clic pe **mai multe informații**. Sunt afișate informații despre setările regulii Inbox în câmpul **parametri** .

Pentru mai multe informații, consultați [determinarea dacă un utilizator a creat o regulă de Inbox](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
