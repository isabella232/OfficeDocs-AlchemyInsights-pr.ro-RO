---
title: E-mailuri lipsă în carantină
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569557"
---
# <a name="missing-emails-in-quarantine"></a>E-mailuri lipsă în carantină"

Administratorii pot [vizualiza, elibera sau șterge aceste mesaje.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Pentru a deschide Centrul de conformitate & securitate, accesați [https://protection.office.com](https://protection.office.com/) . Pentru a deschide direct pagina Carantină, accesați [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Puteți căuta după următoarele valori:  

- **ID mesaj:** Identificatorul unic global al mesajului. Dacă selectați un mesaj în listă, valoarea **Message ID** apare în panoul de ieșire **Detalii** care apare. Administratorii pot utiliza [urmărirea mesajelor](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) pentru a găsi mesajele și valorile corespunzătoare ale Message ID.
- **Adresa de e-mail a expeditorului:** adresa de e-mail a unui singur expeditor.
- **Adresa de e-mail a destinatarului**: adresa de e-mail a unui singur destinatar.
- **Subiect:** Utilizați întregul subiect al mesajului. Căutarea nu este sensibilă la litere mari și mici.

După ce ați introdus criteriile de căutare, faceți clic pe ![ Reîmprospătare ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) buton**Reîmprospătare** pentru a filtra rezultatele.  

Cmdleturile pe care le utilizați pentru a vizualiza și gestionează mesajele și fișierele aflate în carantină sunt:
- [Mesaj de carantină ștergere](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Mesaj de carantină de export](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Mesaj de carantină](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-quarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Rețineți că acest cmdlet este numai pentru mesaje, nu fișiere malware de la ATP pentru SharePoint Online, OneDrive pentru business sau echipe.
- [Mesaj de carantină de lansare](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)