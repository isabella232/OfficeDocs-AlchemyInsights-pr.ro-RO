---
title: Mesaje de e-mail lipsă în carantină
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539836"
---
# <a name="missing-emails-in-quarantine"></a>Mesaje de e-mail lipsă în carantină"

Administratorii pot [vizualiza, lansa sau șterge aceste mesaje.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Pentru a deschide Centrul de & conformitate, accesați [https://protection.office.com](https://protection.office.com/) . Pentru a deschide direct pagina Carantină, accesați [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Puteți să căutați după următoarele valori:  

- **ID mesaj:** identificatorul unic global al mesajului. Dacă selectați un mesaj din listă, valoarea  **ID mesaj**  apare în panoul  **volant**  Detalii care apare. Administratorii pot utiliza urmărirea [mesajelor pentru](/microsoft-365/security/office-365-security/message-trace-scc) a găsi mesajele și valorile ID-ul de mesaj corespunzătoare.
- **Adresa de e-mail** a expeditorului: adresa de e-mail a unui singur expeditor.
- **Adresa de e-mail** a destinatarului: adresa de e-mail a unui singur destinatar.
- **Subiect:** Utilizați întregul subiect al mesajului. Căutarea nu face sensibil la litere mari și mici.

După ce ați introdus criteriile de căutare, faceți clic ![ pe butonul Reîmprospătare ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **reîmprospătare** pentru a filtra rezultatele.

Cmdleturi pe care le utilizați pentru a vizualiza și gestiona mesajele și fișierele din carantină sunt:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Rețineți că acest cmdlet este doar pentru mesaje, nu pentru fișierele malware de la Microsoft Defender pentru Office 365 pentru SharePoint Online, OneDrive pentru business sau Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)