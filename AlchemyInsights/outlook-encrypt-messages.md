---
title: S/MIME în Outlook pe web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772310"
---
# <a name="encrypt-email-messages-in-outlook"></a>Criptarea mesajelor de e-mail în Outlook

Criptarea mesajelor Microsoft 365 este construită în Microsoft Azure Rights Management (Azure RMS), care face parte din Azure Information Protection. Dacă abonamentul include Azure Rights Management sau Azure Information Protection, **nu trebuie să efectuați acțiuni pentru a activa sau a activa manual** serviciul de administrare a drepturilor.

Pe baza feedbackului de la clienți, nu vom mai permite reguli de flux de corespondență Exchange pentru a cripta automat e-mailurile de ieșire care conțin anumite tipuri de informații sensibile din entitatea găzduită în mod implicit. În schimb, vă oferim instrucțiuni detaliate despre modul în care puteți face acest lucru. Pentru detalii suplimentare despre cum să creați o regulă de transport pentru a cripta informațiile sensibile, consultați [acest articol](https://aka.ms/OmeEtr).

- Dacă utilizați Outlook pe web (anterior **OWA**): atunci când compuneți un mesaj de e-mail, pur și simplu faceți clic pe **Protejare** în OWA. Se va aplica permisiunea "nu se redirecționează". Faceți clic pe **modificare permisiune** și alegeți **criptare** pentru a cripta doar mesajul.

- Dacă utilizați **clientul Outlook**: pentru a trimite un mesaj criptat din Outlook 2013 sau 2016 sau Outlook 2016 pentru Mac, selectați **Options**  >  **permisiuni**de opțiuni, apoi selectați opțiunea de protecție de care aveți nevoie.

- Pentru a **cripta automat toate mesajele de e-mail** trimise anumitor destinatari sau organizații partenere externe, trebuie să creați o regulă de transport a fluxului de corespondență în centrul de administrare Exchange. Instrucțiunile detaliate sunt furnizate în [acest articol de asistență](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

