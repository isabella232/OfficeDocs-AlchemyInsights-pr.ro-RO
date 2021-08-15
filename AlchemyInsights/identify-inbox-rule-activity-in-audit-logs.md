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
ms.openlocfilehash: e27c6433c65079af93f2a02a998b7179222336b0cae1149f4196f6fb6558ddac
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976877"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificarea activității regulilor de inbox în jurnalele de auditare

Puteți utiliza căutarea în jurnalul de auditare din Centrul Microsoft 365 de securitate & pentru a vizualiza evenimentele regulilor de inbox (crearea, modificarea și ștergerea regulilor de inbox).

1. Conectați-vă la [Centrul Microsoft 365 conformitate](https://protection.office.com/).

2. Accesați pagina Căutare **în jurnalul**  >  **de auditare.**

3. Selectați intervalul de date în **câmpurile Dată** de început **și Dată de** sfârșit.

4. Sub **Exchange de cutie poștală**, verificați dacă câmpul Activități este setat la **New-InboxRule Create/modify/enable/disable inbox rule**. 

5. Faceți **clic pe Căutare.**

În rezultate, selectați o înregistrare de auditare. În fișa detalii, faceți clic **pe Mai multe informații**. În câmpul Parametri se afișează informații despre setările **regulii** de inbox.

Pentru mai multe informații, consultați [Determinarea dacă un utilizator a creat o regulă de inbox](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
