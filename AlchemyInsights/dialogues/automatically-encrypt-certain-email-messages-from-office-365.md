---
title: Criptarea automată a anumitor mesaje de e-mail din Office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526761"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Criptarea automată a anumitor mesaje de e-mail din Office 365

1. Din [Centrul de administrare Exchange](https://outlook.office365.com/ecp/), alegeți **regulile de > flux de corespondență**. 
2. Faceți clic pe pictograma **nouă (+)** , apoi faceți clic pe **se aplică criptarea mesajelor Office 365 și protecția drepturilor la mesaje**.
3. În **nume**, introduceți un nume pentru regulă, cum ar fi *Criptarea tuturor mesajelor*.
4. În **se aplică această regulă dacă**, alegeți **[se aplică la toate mesajele]**. 
5. Lângă câmpul **fă următorul** , faceți clic pe **Selectare**. 
6. În meniul vertical **șablon RMS** , selectați **criptare**, apoi faceți clic pe **OK**. (Dacă nu vedeți această opțiune, înseamnă că planul nu include criptarea automată. Dar îl puteți adăuga!)
7. Bifați caseta de selectare **auditare regulă cu nivel de severitate** , apoi selectați nivelul dorit. Dacă firma dumneavoastră are obligații contractuale de a trimite toate mesajele de e-mail criptate, vă recomandăm să setați nivelul la **maxim**.
8. Sub **alegere model pentru această regulă**, faceți clic pe **aplicare**. 
9. Alegeți orice selecție opțională (dintr-o listă de selecții opționale pe care le puteți face în acest moment, dintre care multe pot fi lăsate cu setarea implicită pentru simplitate).
10. Faceți clic pe **Salvare**.

> [!IMPORTANT]
> Puteți oricând să reveniți și să editați această regulă mai târziu.

Pentru mai multe informații despre crearea regulilor de criptare, consultați [definirea regulilor de flux de corespondență pentru a cripta mesajele de e-mail în Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

