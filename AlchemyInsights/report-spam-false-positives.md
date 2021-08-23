---
title: Preferați să raportați către Microsoft un spam fals pozitiv?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396627"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Aveți mesaje legitime marcate ca spam?

Este frustrant când un mesaj de e-mail legitim ajunge în folderul E-mail nedorit sau în carantină. Luați în considerare aceste motive cele mai obișnuite pentru rezultatele fals pozitive:

**Înlocuiri de entități găzduite (cel mai comun)** Acest lucru se află în întregime în controlul dvs., pentru a remedia.

Remiterea mesajului pe Microsoft 365 Defender pentru analiza politicilor și regulilor impactului; rescan details are available within minutes.
Revizuiți sau modificați politicile sau regulile, după cum este cazul. 

**Înlocuiri (comune) pentru utilizatorul final** Acest lucru se află în întregime în controlul dvs., pentru a remedia. 

Remiterea mesajului pe Microsoft 365 Defender pentru analiza politicilor și regulilor impactului; rescan details are available within minutes. 

Dacă un mesaj a fost blocat deoarece a fost trimis de la o adresă din lista Expeditori blocați a utilizatorului, anteturile includ Filtrul antispam "SFV:BLK".

**Autentificarea e-mailului expeditorilor** Aceasta se află parțial în controlul dvs. pentru remediere.

Trimiteți mesajul pentru a analiza erorile de autentificare prin e-mail a expeditorului la momentul livrării; rezultatele sunt disponibile în termen de o zi. 

Dacă dețineți infrastructura de expediere, revizuiți cum să o aliniați cu SPF, DKIM și DMARC, pentru a vă asigura că sistemele de e-mail de destinație au încredere în mesajele trimise din domeniul dvs. Alternativ, contactați expeditorii pentru a vă adresa configurațiilor DNS.

**Filtrarea bazelor Microsoft** Aceasta se află parțial în controlul dvs. pentru remediere.

Trimiteți mesajul și raportați mesajul ca sigur; rezultatele rescan sunt disponibile în termen de o zi. Utilizați Lista de entități găzduite/blocare atunci când nu sunteți de acord cu filtrarea, în anumite situații. Cu toate acestea, nu trebuie să omiteți filtrarea definitivă Microsoft. 

Pentru mai multe informații, consultați:

- Permiteți utilizatorilor finali să remită mesaje la Microsoft. Microsoft utilizează aceste remiteri pentru a îmbunătăți eficiența tehnologiilor de protecție a e-mailului și apar în rapoartele de remitere pe care să le utilizați ca indicație de actualizare a politicilor. 

- Pentru a urmări un scurt videoclip despre remiterea mesajelor pentru analiză, consultați [Remiterea mesajelor pentru analiză.](https://go.microsoft.com/fwlink/?linkid=2166435)

- [Utilizați Remiterea de către administrator pentru a remite suspect de spam, mesaje phish, URL-uri și fișiere la Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Gestionarea listei de permitere/blocare pentru entitatea găzduită](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Anteturile mesajelor antispam Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Protecția antispam de ieșire în EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)