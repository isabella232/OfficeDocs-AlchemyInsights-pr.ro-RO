---
title: Mutarea automată a mesajelor de e-mail în cutia poștală de arhivă
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
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527102"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Mutarea automată a mesajelor de e-mail în cutia poștală de arhivă

Iată cum să configurați o politică pentru a muta automat e-mailul vechi al unui utilizator în cutia poștală de arhivă:

1. Accesați Arhiva [**de**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **guvernanță a datelor** de conformitate &  >   pentru a verifica dacă a fost activată o cutie poștală de arhivă pentru utilizator. Dacă nu are, faceți clic pe **Activare** , apoi pe **Da** în caseta avertisment.
2. Accesați [**Centrul de administrare Exchange > gestionarea conformității > etichetele de retenție**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Alegeți pictograma +, apoi alegeți **se aplică automat la întreaga cutie poștală**.
4. Atribuiți un nume etichetei de retenție și alegeți **Mutare în arhivă**. Pentru perioada de retenție, introduceți ora dorită, cum ar fi 90 zile. Faceți clic pe **Salvare**.
5. Acum creați o politică de retenție: alegeți **politici de retenție**, alegeți pictograma pentru a adăuga o politică nouă.
6. Atribuiți un nume politicii de retenție, apoi faceți clic și defilați pentru a găsi și a adăuga eticheta de retenție pe care tocmai ați creat-o. Faceți clic pe **Salvare**.
7. În cele din urmă, aplicați Politica de retenție la cutia poștală a utilizatorului: tot în centrul de administrare Exchange, accesați  >  **cutiile poștale** destinatari. Alegeți toți utilizatorii la care doriți să aplicați politica, apoi alegeți **Editare** (pictograma creion).
8. În caseta de dialog, faceți clic pe **caracteristici cutie poștală**. Sub **politică de retenție**, aplicați politica pe care tocmai ați creat-o > **Salvare**.
9. Pentru instrucțiuni pentru aplicarea politicii pentru toți utilizatorii, consultați [aplicarea unei politici de retenție la cutiile poștale](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
