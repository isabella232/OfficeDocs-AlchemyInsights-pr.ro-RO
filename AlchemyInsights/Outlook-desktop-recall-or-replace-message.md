---
title: Outlook desktop retragerea sau înlocuirea unui mesaj de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664002"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Retragerea sau înlocuirea unui mesaj de e-mail Outlook

- Ca administrator, puteți retrage **mesaje în numele utilizatorilor care utilizează PowerShell**. Nu puteți retrage mesaje din centrul de administrare.
- Puteți să **rememorați doar mesajele care sunt trimise persoanelor din organizația dvs**. În cazul în care mesajul a fost trimis la o adresă Gmail, de exemplu, nu vă puteți retrage memoria.
- Puteți să **rememorați doar mesajele trimise din Outlook 2016 pe PC**. Dacă un utilizator trimite un mesaj utilizând Outlook pentru Mac sau Outlook pe web, nu vă puteți retrage memoria.

Pentru retragerea sau înlocuirea unui mesaj de e-mail:

1. În panoul de foldere din partea stângă a ferestrei Outlook, selectați folderul Elemente trimise.
1. Faceți dublu clic pe mesajul pe care doriți să-l rememorați pentru a-l deschide.
1. Selectați fila **mesaj** , apoi faceți clic pe **acțiuni**  >  **retragerea acestui mesaj**.
1. Selectați **ștergeți copiile necitite ale acestui mesaj** sau **Ștergeți copii necitite și înlocuiți cu un mesaj nou**, apoi selectați **OK**.
1. Dacă trimiteți un mesaj de înlocuire, compuneți mesajul, apoi selectați **Trimitere**.
1. Succesul sau nereușita unui mesaj retras depinde de setările destinatarului în Outlook. Pentru pașii necesari pentru a verifica retragerea, consultați [acest articol](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Căutarea și ștergerea mesajelor de e-mail din organizație

- Dacă nu sunteți administrator global, contul dumneavoastră trebuie să fie adăugat la rolul managerului eDiscovery sau la rolul de gestionare a căutării conformității pentru a căuta mesaje. Pentru a șterge mesaje, va trebui să vă asociați grupului de roluri pentru gestionarea organizației sau rolul de gestionare a căutării și eliminării. Permisiunile pentru aceste roluri sunt atribuite în [Centrul de securitate și conformitate](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Creați o căutare de conținut](https://docs.microsoft.com/microsoft-365/compliance/content-search) pentru a găsi mesajul de șters.
- [Conectați-vă la centrul de securitate și conformitate PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Dacă utilizați autentificarea multi-factor, consultați [conectarea la Microsoft 365 Security și la centrul de conformitate PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).