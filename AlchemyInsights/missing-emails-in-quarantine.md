---
title: Mesaje de e-mail lipsă în carantină
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673726"
---
# <a name="missing-emails-in-quarantine"></a>Mesaje de e-mail lipsă în carantină "

Administratorii pot să [vizualizeze, să lanseze sau să șteargă aceste mesaje.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Pentru a deschide centrul de conformitate &, accesați [https://protection.office.com](https://protection.office.com/) . Pentru a deschide direct pagina carantină, accesați [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Puteți căuta după valorile următoare:  

- **ID mesaj**: identificatorul unic global al mesajului. Dacă selectați un mesaj în listă, valoarea  **ID mesaj**  apare în panoul flyout  **Detalii**  care apare. Administratorii pot utiliza [urmărirea](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) mesajelor pentru a găsi mesaje și valorile corespunzătoare pentru ID-ul mesajului.
- **Adresa de E-mail a expeditorului**: adresa de E-mail a unui singur expeditor.
- **Adresa de E-mail a destinatarului**: adresa de E-mail a unui singur destinatar.
- **Subiect**: utilizați întregul subiect al mesajului. Căutarea nu este sensibilă la litere mari și mici.

După ce ați introdus criteriile de căutare, faceți clic pe Reîmprospătare buton reîmprospătare ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** pentru a filtra rezultatele.  

Cmdleturile pe care le utilizați pentru a vizualiza și a gestiona mesajele și fișierele în carantină sunt:
- [Ștergere-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): rețineți că acest cmdlet este doar pentru mesaje, nu pentru fișiere malware din ATP pentru SharePoint Online, OneDrive pentru Business sau teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)