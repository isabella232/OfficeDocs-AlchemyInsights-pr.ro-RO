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
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511520"
---
# <a name="encrypt-email-messages-in-outlook"></a>Criptarea mesajelor de e-mail în Outlook

Microsoft 365 mesaj criptare este construit pe Microsoft Azure Rights Management (Azure RMS), care face parte din Azure Information Protection. Dacă abonamentul include Azure Rights Management sau Azure Information Protection, **nu este necesar să efectuați nicio acțiune pentru a activa sau activa manual** Serviciul de gestionare a drepturilor.

Pe baza feedback-ului clientului, nu vom mai permite regulilor fluxului de corespondență Exchange să cripteze automat e-mailul de ieșire care conține anumite tipuri de informații sensibile din entitatea găzduită în mod implicit. În schimb, oferim instrucțiuni detaliate cu privire la modul în care puteți face acest lucru voi înșivă. Pentru detalii suplimentare despre se creează o regulă de transport pentru a cripta informațiile sensibile, consultați [acest articol](https://aka.ms/OmeEtr).

- Dacă utilizați Outlook pe Web (anterior **OWA**): Atunci când compuneți un mesaj de poștă electronică, pur și simplu faceți clic pe **Protejaîn** OWA. Acest lucru se va aplica "Nu înainte" permisiunea. Faceți clic pe **Modificare permisiune** și **alegeți Criptare** pentru a cripta numai mesajul.

- Dacă utilizați **clientul Outlook**: Pentru a trimite un mesaj criptat din Outlook 2013 sau 2016 sau Outlook 2016 pentru Mac, selectați **Permisiuni de opțiuni**, apoi  >  **Permissions**selectați opțiunea de protecție de care aveți nevoie.

- Pentru a **cripta automat toate e-mailurile** trimise anumitor destinatari sau organizații partenere externe, trebuie să creați o regulă de transport flux de corespondență în Centrul de administrare Exchange. Instrucțiuni detaliate sunt furnizate în [acest articol de asistență](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

