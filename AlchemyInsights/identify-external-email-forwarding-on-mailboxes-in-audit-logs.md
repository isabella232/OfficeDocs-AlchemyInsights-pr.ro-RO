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
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028761"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificarea atunci când este configurată redirecționarea e-mailului extern pentru cutiile poștale

Atunci când Microsoft 365 configurează redirecționarea externă a e-mailurilor pentru o cutie poștală, activitatea este auditată ca parte a cmdletului **Set-Mailbox.** Puteți vedea activitatea utilizând căutarea în jurnalul de auditare din Centrul de & conformitate.

1. Conectați-vă la [Centrul Microsoft 365 conformitate](https://protection.office.com/).

2. Accesați pagina Căutare **în jurnalul**  >  **de auditare.**

3. Selectați intervalul de date în **câmpurile Dată** de început **și Dată de** sfârșit. Nu trebuie să specificați un nume de utilizator. Verificați **dacă câmpul** Activități este setat la **Afișați rezultate pentru toate activitățile.**

4. Faceți **clic pe Căutare.**

În rezultate, faceți clic **pe Filtrare rezultate** și tastați **Set-Mailbox** în caseta de filtrare de activitate. Selectați o înregistrare de auditare în rezultate. În **fișa Detalii,** faceți clic **pe Mai multe informații**. Trebuie să priviți detaliile fiecărei înregistrări de auditare pentru a determina dacă activitatea este corelată cu redirecționarea e-mailului.

- **ObjectId:** Valoarea alias a cutiei poștale care a fost modificată.

- **Parametri:** _RedirecționareaSmtpAddress indică_ adresa de e-mail țintă.

- **UserId:** Utilizatorul care a configurat redirecționarea e-mailului în cutia poștală **din câmpul ObjectId.**

Pentru mai multe informații, consultați [Determinarea cine a configurat redirecționarea e-mailului pentru o cutie poștală.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
