---
title: Mutarea automată a mesajelor de e-mail în cutia poștală de arhivare
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
- "3100008"
- "7217"
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059238"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Mutarea automată a mesajelor de e-mail în cutia poștală de arhivare

Iată cum să configurați o politică pentru a muta automat e-mailul vechi al unui utilizator în cutia poștală de arhivare:

1. Accesați Arhiva [**de & de conformitate a**](https://go.microsoft.com/fwlink/p/?linkid=2077143)datelor pentru a verifica dacă a fost activată o cutie  >    >   poștală de arhivare pentru utilizator. Dacă nu a făcut acest lucru, faceți **clic pe** **Activare, apoi** pe Da în caseta de avertisment.
2. Accesați Centrul de [**administrare Exchange centrul de administrare > conformitatea și > de conservare.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Alegeți pictograma +, apoi alegeți **Se aplică automat la întreaga cutie poștală**.
4. Atribuiți un nume etichetei de retenție și **alegeți Mutați în Arhivă.** Pentru perioada de reținere, introduceți ora dorită, cum ar fi 90 de zile. Faceți clic pe **Salvare**.
5. Acum creați o politică de retenție: **alegeți politici de retenție**, alegeți pictograma pentru a adăuga o politică nouă.
6. Atribuiți un nume politicii de retenție, apoi faceți clic și defilați pentru a găsi și a adăuga eticheta de retenție pe care tocmai ați creat-o. Faceți clic pe **Salvare**.
7. În sfârșit, aplicați politica de retenție pentru cutia poștală a utilizatorului: tot în centrul Exchange, accesați **cutiile poștale ale**  >  **destinatarilor.** Alegeți toți utilizatorii pentru care doriți să aplicați politica, apoi alegeți **Editare** (pictograma creion).
8. În caseta de dialog, faceți clic pe caracteristici **cutie poștală**. Sub Politică **de retenție**, aplicați politica pe care tocmai ați creat-> **Salvare**.
9. Pentru instrucțiuni privind aplicarea politicii pentru toți utilizatorii, consultați Aplicarea unei politici de [retenție pentru cutiile poștale.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
