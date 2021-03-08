---
title: Criptarea automată a anumitor mesaje de e-mail Office 365
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526739"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Criptarea automată a anumitor mesaje de e-mail Office 365

Puteți cripta automat mesajele pe care utilizatorii le trimit anumitor persoane sau organizații externe. Pentru a face acest lucru, efectuați pașii următori:

1. Din [Centrul de administrare Exchange](https://outlook.office365.com/ecp/), alegeți **regulile de > flux de corespondență**. 
2. Faceți clic pe pictograma **nouă (+)** , apoi faceți clic pe **se aplică criptarea mesajelor Office 365 și protecția drepturilor la mesaje**.
3. În **nume**, introduceți un nume pentru regulă, cum ar fi *Criptarea mesajelor trimise către DrToniRamos@gmail.com*.
4. În **se aplică această regulă dacă**, alegeți **> destinatar este această persoană**. 
5. În fereastra **Selectare membri** , selectați numele persoanei la care doriți să se aplice regula de criptare, apoi faceți clic pe **Adăugare**. 
6. Când ați terminat de adăugat utilizatori, faceți clic pe **OK**.
7. Lângă câmpul **fă următorul** , faceți clic pe **Selectare**. 
8. În meniul vertical **șablon RMS** , selectați **criptare**, apoi faceți clic pe **OK**. (Dacă nu vedeți această opțiune, înseamnă că planul nu include criptarea automată. Dar îl puteți adăuga!)
9. Alegeți orice selecție opțională (dintr-o listă de selecții opționale pe care le puteți face în acest moment, dintre care multe pot fi lăsate cu setarea implicită pentru simplitate).
10. Faceți clic pe **Salvare**.

> [!IMPORTANT]
> Puteți oricând să reveniți și să editați această regulă mai târziu.

Pentru mai multe informații despre crearea regulilor de criptare, consultați [definirea regulilor de flux de corespondență pentru a cripta mesajele de e-mail în Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

