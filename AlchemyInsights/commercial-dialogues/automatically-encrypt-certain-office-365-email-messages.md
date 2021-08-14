---
title: Criptați automat anumite mesaje Office 365 e-mail
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 8ae1c6853f41790efc3b24a9dc696bccf8385967d8c9219a1200e287e6ce32a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53949579"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Criptați automat anumite mesaje Office 365 e-mail

Puteți cripta automat mesajele pe care utilizatorii le trimit anumitor persoane sau organizații externe. Pentru a face acest lucru, efectuați pașii următori:

1. Din centrul [de Exchange , alegeți](https://outlook.office365.com/ecp/)Reguli pentru **fluxul de > corespondență**. 
2. Faceți **clic pe pictograma Nou (+),** apoi faceți clic **pe Office 365 Message Encryption și drepturi de protecție la mesaje.**
3. În **Nume,** introduceți un nume pentru regulă, cum ar fi *Criptați mesajele trimise la DrToniRamos@gmail.com*.
4. În **Se aplică această regulă dacă**, **alegeți Destinatarul > este această persoană**. 
5. În fereastra **Selectare membri,** selectați numele persoanei la care doriți să se aplice regula de criptare, apoi faceți clic pe **Adăugare**. 
6. După ce terminați de adăugat utilizatori, faceți clic **pe OK.**
7. Lângă câmpul **Faceți următoarele, faceți** clic **pe Selectare.** 
8. În meniul **vertical al șablonului RMS,** selectați **Criptare**, apoi faceți clic pe **OK.** (Dacă nu vedeți această opțiune, înseamnă că planul dvs. nu include criptarea automată. Dar îl puteți adăuga!)
9. Alegeți orice selecție opțională (dintr-o listă de selecții opționale pe care le puteți face în acest moment, dintre care multe pot fi rămase cu setarea implicită pentru simplitate).
10. Faceți clic pe **Salvare**.

> [!IMPORTANT]
> Puteți oricând să reveniți și să editați această regulă mai târziu.

Pentru mai multe informații despre crearea de reguli pentru criptare, consultați Definirea regulilor de [flux de corespondență pentru a cripta mesajele de e-mail Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

