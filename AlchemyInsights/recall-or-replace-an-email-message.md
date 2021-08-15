---
title: Retragerea sau înlocuirea unui mesaj de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024398"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Retragerea sau înlocuirea unui mesaj de e-mail Microsoft 365

- Puteți retragerea **doar a mesajelor care sunt trimise persoanelor din organizația dvs.** De exemplu, dacă mesajul a fost trimis la o adresă Gmail, nu-l mai puteți aminti.
- Puteți retragerea **doar a mesajelor trimise Outlook pentru PC.** Dacă un utilizator trimite un mesaj utilizând Outlook pentru Mac sau Outlook pe web, nu îl puteți reaminti.
- Ca administrator al entității găzduite, puteți retragerea mesajelor în numele utilizatorilor utilizând **PowerShell** (Pentru mai multe informații, consultați: Căutarea și ștergerea mesajelor de [e-mail).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- Nu puteți retragerea mesajelor din centrul de administrare. Defilați în jos la "Căutați și ștergeți mesaje de e-mail din organizația dvs." pentru mai multe informații.

**Retragerea sau înlocuirea unui mesaj de e-mail trimis**

1. În panoul de foldere din partea stângă a ferestrei Outlook de mesaje, alegeți folderul Elemente trimise.
2. Deschideți mesajul pe care doriți să îl retragereați. Trebuie să faceți dublu clic pentru a deschide mesajul. Selectarea mesajului astfel încât să apară în panoul de citire nu vă va permite să retragerea mesajului.
3. Din fila Mesaj, selectați **Acțiuni Retragerea**  >  **acestui mesaj**.
4. Alegeți **Ștergeți copiile necitite ale acestui mesaj sau** Ștergeți **copiile necitite și înlocuiți cu un** mesaj nou , apoi selectați **OK**.
5. Dacă trimiteți un mesaj de înlocuire, compuneți mesajul, apoi selectați **Trimitere**.
6. Reușita sau eșecul retragerea unui mesaj depinde de setările din Outlook.

Pentru mai multe informații, inclusiv despre cum să verificați retragerea, consultați Retragerea sau [înlocuirea unui mesaj de e-mail trimis.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Pentru a căuta și a șterge mesaje de e-mail*** din organizația dvs., este mai simplu dacă fiți administrator global. Dacă nu sunt administrator global, contul dvs. trebuie să fie adăugat la grupul de roluri Manager pentru descoperirea informațiilor electronic sau la rolul de gestionare a căutării de conformitate. Pentru a șterge mesaje, va trebui să vă asociați grupului de roluri Gestionare organizație sau rolului de gestionare a căutării și ștergerii definitiv. Permisiunile pentru aceste roluri sunt atribuite în Centrul [de & conformitate](https://protection.office.com/).

1. [Creați o căutare de conținut](https://docs.microsoft.com/microsoft-365/compliance/content-search) pentru a găsi mesajul de șters.
2. [Conectare la PowerShell din Centrul de & securitate și conformitate.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

Dacă utilizați MFA (Multi-Factor Authentication), consultați autentificarea prin mai multe metode Conectare [Microsoft 365 Security & PowerShell utilizând Multi-Factor Authentication.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
