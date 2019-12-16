---
title: S/MIME în Outlook pe web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053237"
---
# <a name="encrypt-email-messages-in-outlook"></a>Criptarea mesajelor de e-mail în Outlook

Office 365 mesaj Encryption este construit pe Microsoft Azure Rights Management (Azure RMS), care face parte din protecție informații Azure. Dacă abonamentul include Azure Rights Management sau Azure Information Protection, **nu trebuie să efectuați nicio acțiune pentru a activa sau activa manual** serviciul de administrare a drepturilor.

Pe baza feedback-ului clientului, nu vom mai permite regulilor de flux de corespondență Exchange să cripteze automat e-mailul de ieșire care conține anumite tipuri de informații sensibile în entitatea găzduită în mod implicit. În schimb, oferim instrucțiuni detaliate despre puteți face acest lucru. Pentru detalii suplimentare despre să creați o regulă de transport pentru a cripta informații sensibile, consultați [acest articol](https://aka.ms/OmeEtr).

- Dacă utilizați Outlook pe web (fostă **OWA**): Când compuneți un mesaj de poștă electronică, pur și simplu faceți clic pe **Protejare** în OWA. Acest lucru va aplica permisiunea "nu redirecționați". Faceți clic pe **modificare permisiune** și alegeți **criptare** pentru a cripta numai mesajul.

- Dacă utilizați **clientul Outlook**: pentru a trimite un mesaj criptat din Outlook 2013 sau 2016 sau Outlook 2016 pentru Mac, selectați **Opțiuni** > **permisiuni**, apoi selectați opțiunea de protecție de care aveți nevoie.

- Pentru a **cripta automat toate mesajele de poștă electronică** trimise anumitor destinatari sau organizații partenere externe, trebuie să creați o regulă de transport flux de corespondență în centrul de administrare Exchange. Instrucțiuni detaliate sunt furnizate în [acest articol de asistență](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

