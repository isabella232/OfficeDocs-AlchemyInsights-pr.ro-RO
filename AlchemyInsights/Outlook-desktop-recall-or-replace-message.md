---
title: Outlook desktop amintesc sau înlocui un mesaj de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36496123"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Retragerea sau înlocuirea unui mesaj de e-mail Outlook

- Ca admin, puteți **aminti mesaje în numele utilizatorilor folosind PowerShell**. Nu vă puteți aminti mesajele de la centrul de administrare.
- Puteți **aminti doar mesajele care sunt trimise către persoane din organizația dvs**. Dacă mesajul a fost trimis la o adresă Gmail, de exemplu, nu vă puteți aminti.
- Puteți **aminti doar mesajele trimise din Outlook 2016 pe PC**. Dacă un utilizator trimite un mesaj utilizând Outlook pentru Mac sau Outlook pe web, nu vă puteți aminti.

Pentru a rechema sau a înlocui un mesaj e-mail:

1. În panoul de foldere din partea stângă a ferestrei Outlook, selectați folderul Elemente trimise.
1. Faceți dublu clic pe mesajul pe care doriți să-l reamintiți pentru a-l deschide.
1. Selectați fila **mesaj** , apoi selectați **acțiuni** > **reamintiți acest mesaj**.
1. Selectați **ștergeți copiile necitite ale acestui mesaj** sau **ștergeți copiile necitite și înlocuiți cu un mesaj nou**, apoi selectați **OK**.
1. Dacă trimiteți un mesaj de înlocuire, compuneți mesajul, apoi selectați **Trimitere**.
1. Succesul sau eșecul unui mesaj de retragere depinde de setările destinatarului în Outlook. Pentru pași pentru a verifica pe Recall, a se vedea [acest articol](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Căutați și ștergeți mesajele de e-mail din organizația dvs.

- Dacă nu sunteți administrator global, contul trebuie adăugat la rolul eDiscovery Manager sau la rolul de gestionare a căutării de conformitate pentru a căuta mesaje. Pentru a șterge mesajele, va trebui să vă alăturați grupului de roluri Gestionare organizație sau rolului de gestionare căutare și Golire. Permisiunile pentru aceste roluri sunt atribuite în [Centrul de securitate și conformitate](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Creați o căutare de conținut](https://docs.microsoft.com/office365/securitycompliance/content-search) pentru a găsi mesajul de șters.
- [Conectați-vă la centrul de securitate și conformitate PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Dacă utilizați autentificarea multi-factor, consultați [conectarea la Office 365 securitate și centrul de conformitate PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).