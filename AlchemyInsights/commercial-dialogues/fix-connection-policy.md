---
title: Remedierea politicii de conexiune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988138"
---
# <a name="fix-connection-policy"></a>Remedierea politicii de conexiune

Mesajul de e-mail a fost marcat ca sigur și livrat în inboxul utilizatorului, deoarece adresa IP de expediere a fost marcată ca sigură în politica Filtru de conexiune. Pentru a revizui politica, acțiunile următoare:

1. Accesați Centrul de [Office 365 securitate &](https://go.microsoft.com/fwlink/p/?linkid=2077143), apoi accesați Politica de gestionare a  >  **amenințărilor**  >  [Antispam.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Pe fila **Particularizate,** selectați Politica **de filtrare a conexiunii**, apoi selectați **Editați politica**.
3. Revizuiți **lista de adrese IP permisă.** Vedeți dacă **Seif** este activată.

    > [!NOTE]
    > Microsoft se abonează la surse terțe ale expeditorilor de încredere. Dacă **Seif este** activată, acești expeditori de încredere nu sunt marcați din greșeală ca spam. Vă recomandăm să selectați această opțiune, deoarece va reduce numărul de rezultate fals pozitive (mesaje bune clasificate ca spam) pe care le primiți.
