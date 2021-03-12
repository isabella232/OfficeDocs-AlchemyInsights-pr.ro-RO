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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750603"
---
# <a name="fix-connection-policy"></a>Remedierea politicii de conexiune

Mesajul de e-mail a fost marcat în siguranță și livrat în inboxul utilizatorului, deoarece adresa IP de trimitere a fost marcată în siguranță în Politica de filtrare a conexiunii. Pentru a revizui politica, procedați astfel:

1. Accesați centrul de [conformitate Office 365 Security &](https://go.microsoft.com/fwlink/p/?linkid=2077143), apoi accesați Politica de **gestionare a amenințărilor**  >    >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Pe fila **particularizat** , selectați Politica de **filtrare a conexiunii**, apoi selectați **Editare politică**.
3. Revizuiți lista de **permisiuni IP** . Vedeți dacă este activată **lista sigură** .

    > [!NOTE]
    > Microsoft se abonează la sursele terților de expeditori de încredere. Dacă este activată **lista sigură** , acești expeditori de încredere nu sunt marcați din greșeală ca spam. Vă recomandăm să selectați această opțiune, deoarece va reduce numărul de fals pozitive (corespondență bună clasificat ca spam) pe care îl primiți.
