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
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010736"
---
# <a name="encrypt-email-messages-in-outlook"></a>Criptarea mesajelor de e-mail Outlook

Microsoft 365 Criptarea mesajelor este încorporată în Microsoft Azure Rights Management (Azure RMS), care face parte din Azure Information Protection. Dacă abonamentul dvs. include Azure Rights Management sau Azure Information Protection, nu trebuie să luați nicio acțiune pentru a activa sau activa **manual** Serviciul de administrare a drepturilor.

Pe baza feedbackului de la clienți, nu vom mai permite reguli Exchange fluxului de corespondență pentru Exchange cripta automat e-mailurile de ieșire care conțin anumite tipuri de informații sensibile în entitatea dvs. găzduită în mod implicit. În schimb, oferim instrucțiuni detaliate despre cum puteți face acest lucru. Pentru detalii suplimentare despre cum să creați o regulă de transport pentru a cripta informațiile sensibile, [consultați acest articol.](https://aka.ms/OmeEtr)

- Dacă utilizați Outlook pe web (anterior **OWA**): atunci când compuneți un mesaj de e-mail, pur și simplu faceți clic **pe Protejare** în OWA. Acest lucru va aplica permisiunea "Nu se redirecționează". Faceți **clic pe Modificare** permisiune și **alegeți** Criptare pentru a cripta doar mesajul.

- Dacă se **utilizează Outlook:** Pentru a trimite un mesaj criptat din Outlook 2013, 2016 sau Outlook 2016 pentru Mac, selectați Permisiuni opțiuni , apoi selectați opțiunea de protecție de care aveți  >  nevoie.

- Pentru a **cripta automat toate mesajele** de e-mail trimise anumitor destinatari sau organizațiilor partenere externe, trebuie să creați o regulă de transport flux de corespondență în Centrul de administrare Exchange. Instrucțiunile detaliate sunt furnizate [în acest articol de asistență.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

