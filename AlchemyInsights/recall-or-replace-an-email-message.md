---
title: Rechemarea sau înlocuirea unui mesaj de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509468"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Rechemarea sau înlocuirea unui mesaj de e-mail în Microsoft 365

- Aveți posibilitatea **să reamintiți numai mesajele care sunt trimise persoanelor din organizația dvs.** Dacă mesajul a fost trimis la o adresă Gmail, de exemplu, nu-l puteți rechema.
- Aveți posibilitatea să **rechemați numai mesajele trimise din Outlook 2016 pentru PC**. Dacă un utilizator trimite un mesaj utilizând Outlook pentru Mac sau Outlook pe web, nu-l puteți rechema.
- Dacă sunteți administrator, puteți **rechema mesajele în numele utilizatorilor utilizând PowerShell**. Nu vă puteți aminti mesajele din centrul de administrare. Derulați în jos la "Căutați și ștergeți mesajele de e-mail din organizația dvs." pentru mai multe informații.

**Regăsirea sau înlocuirea unui mesaj de e-mail pe care l-ați trimis**

1. În panoul de foldere din partea stângă a ferestrei Outlook, alegeți folderul Elemente trimise.
2. Deschideți mesajul pe care doriți să-l rechemați. Trebuie să faceți dublu clic pentru a deschide mesajul. Selectarea mesajului astfel încât să apară în panoul de citire să nu vă permită să rechemați mesajul.
3. Din fila Mesaj, **selectați**  >  **Acțiuni Rechemarea acestui mesaj**.
4. Selectați **Ștergere copii necitite ale acestui mesaj** sau Ștergere copii **necitite și înlocuire cu un mesaj nou**, apoi selectați **OK**.
5. Dacă trimiteți un mesaj de înlocuire, compuneți mesajul, apoi selectați **Trimitere**.
6. Succesul sau eșecul unei rechemări a mesajului depinde de setările destinatarilor din Outlook.

Pentru mai multe informații, inclusiv să verificați rechemarea, consultați [Reamintirea sau înlocuirea unui mesaj de e-mail pe care l-ați trimis](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Căutarea și ștergerea mesajelor de e-mail în organizația dvs.*** Pentru a căuta și a șterge mesajele de e-mail din organizația dvs., este mai ușor dacă sunteți administrator global. Dacă nu sunteți administrator global, contul trebuie adăugat la grupul de roluri eDiscovery Manager sau la rolul de gestionare a Căutării de conformitate. Pentru a șterge mesajele, va trebui să vă asociați la grupul de roluri Gestionare organizație sau la rolul de gestionare căutare și golire. Permisiunile pentru aceste roluri sunt atribuite în [centrul de securitate & conformitate](https://protection.office.com/).

1. [Creați o căutare de conținut](https://docs.microsoft.com/microsoft-365/compliance/content-search) pentru a găsi mesajul de șters.
2. [Conectarea la Centrul de conformitate Security & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Dacă utilizați MAE, consultați [Conectarea la Microsoft 365 security & Compliance Center PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
