---
title: Outlook Desktop amintesc sau înlocui un mesaj de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502331"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Rechemarea sau înlocuirea unui mesaj de e-mail Outlook

- În calitate de administrator, puteți **rechema mesajele în numele utilizatorilor care utilizează PowerShell**. Nu vă puteți aminti mesajele din centrul de administrare.
- Aveți posibilitatea **să reamintiți numai mesajele care sunt trimise persoanelor din organizația dvs.** Dacă mesajul a fost trimis la o adresă Gmail, de exemplu, nu-l puteți rechema.
- Puteți **rechema numai mesajele trimise din Outlook 2016 pe PC**. Dacă un utilizator trimite un mesaj utilizând Outlook pentru Mac sau Outlook pe web, nu-l puteți rechema.

Pentru a reaminti sau a înlocui un mesaj de e-mail:

1. În panoul de foldere din partea stângă a ferestrei Outlook, selectați folderul Elemente trimise.
1. Faceți dublu clic pe mesajul pe care doriți să-l rechemați pentru a-l deschide.
1. Selectați fila **Mesaj,** apoi **selectați**  >  **Acțiuni Rechemarea acestui mesaj**.
1. Selectați **Ștergere copii necitite ale acestui mesaj** sau Ștergere copii **necitite și înlocuire cu un mesaj nou**, apoi selectați **OK**.
1. Dacă trimiteți un mesaj de înlocuire, compuneți mesajul, apoi selectați **Trimitere**.
1. Succesul sau eșecul unei rechemări a mesajului depinde de setările destinatarului în Outlook. Pentru pași pentru a verifica rechemarea, consultați [acest articol](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Căutarea și ștergerea mesajelor de e-mail în organizația dvs.

- Dacă nu sunteți administrator global, contul trebuie adăugat la rolul eDiscovery Manager sau la rolul de gestionare a căutării de conformitate pentru a căuta mesaje. Pentru a șterge mesajele, va trebui să vă asociați la grupul de roluri Gestionare organizație sau la rolul de gestionare căutare și golire. Permisiunile pentru aceste roluri sunt atribuite în [centrul de securitate și conformitate](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Creați o căutare de conținut](https://docs.microsoft.com/microsoft-365/compliance/content-search) pentru a găsi mesajul de șters.
- [Conectarea la Centrul de securitate și conformitate PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Dacă utilizați autentificarea multi-factor, consultați [Conectarea la Microsoft 365 security and Compliance Center PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).