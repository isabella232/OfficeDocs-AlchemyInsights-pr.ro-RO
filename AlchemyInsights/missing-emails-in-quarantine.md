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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831746"
---
# <a name="missing-emails-in-quarantine"></a>Mesaje de e-mail lipsă în carantină"

Administratorii pot [vizualiza, lansa sau șterge aceste mesaje.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Pentru a deschide Centrul de & conformitate, accesați [https://protection.office.com](https://protection.office.com/) . Pentru a deschide direct pagina Carantină, accesați [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Puteți să căutați după următoarele valori:  

- **ID mesaj:** identificatorul unic global al mesajului. Dacă selectați un mesaj din listă, valoarea  **ID mesaj**  apare în panoul  **volant**  Detalii care apare. Administratorii pot utiliza urmărirea [mesajelor pentru](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) a găsi mesajele și valorile ID-ul de mesaj corespunzătoare.
- **Adresa de e-mail** a expeditorului: adresa de e-mail a unui singur expeditor.
- **Adresa de e-mail** a destinatarului: adresa de e-mail a unui singur destinatar.
- **Subiect:** Utilizați întregul subiect al mesajului. Căutarea nu face sensibil la litere mari și mici.

După ce ați introdus criteriile de căutare, faceți clic ![ pe butonul Reîmprospătare ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **reîmprospătare** pentru a filtra rezultatele.  

Cmdleturi pe care le utilizați pentru a vizualiza și gestiona mesajele și fișierele din carantină sunt:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Rețineți că acest cmdlet este doar pentru mesaje, nu pentru fișierele malware de la ATP pentru SharePoint Online, OneDrive pentru business sau Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)