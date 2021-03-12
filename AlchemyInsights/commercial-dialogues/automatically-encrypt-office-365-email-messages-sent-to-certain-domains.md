---
title: Criptarea automată a mesajelor de e-mail Office 365 trimise anumitor domenii
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749303"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Criptarea automată a mesajelor de e-mail Office 365 trimise anumitor domenii

1. Din [Centrul de administrare Exchange](https://outlook.office365.com/ecp/), alegeți **regulile de > flux de corespondență**. 
2. Faceți clic pe pictograma **nouă (+)** , apoi faceți clic pe **se aplică criptarea mesajelor Office 365 și protecția drepturilor la mesaje**.
3. În **nume**, introduceți un nume pentru regulă, cum ar fi *Criptarea mesajelor trimise către contoso.com*.
4. În **se aplică această regulă dacă**, alegeți **domeniul > destinatarului**. 
5. Introduceți numele domeniului, cum ar fi **contoso.com**.
6. Faceți clic pe pictograma **Add (+)** , apoi faceți clic pe **OK**.
7. Lângă câmpul **fă următorul** , faceți clic pe **Selectare**. 
8. În meniul vertical **șablon RMS** , selectați **criptare**, apoi faceți clic pe **OK**. (Dacă nu vedeți această opțiune, înseamnă că planul nu include criptarea automată. Dar îl puteți adăuga!)
9. Alegeți orice selecție opțională (dintr-o listă de selecții opționale pe care le puteți face în acest moment, dintre care multe pot fi lăsate cu setarea implicită pentru simplitate).
10. Faceți clic pe **Salvare**.

> [!IMPORTANT]
> Puteți oricând să reveniți și să editați această regulă mai târziu.

Pentru mai multe informații despre crearea regulilor de criptare, consultați [definirea regulilor de flux de corespondență pentru a cripta mesajele de e-mail în Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)