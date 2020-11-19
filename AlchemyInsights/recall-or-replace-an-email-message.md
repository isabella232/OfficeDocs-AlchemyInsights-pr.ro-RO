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
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353518"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Retragerea sau înlocuirea unui mesaj de e-mail în Microsoft 365

- Puteți să **rememorați doar mesajele care sunt trimise persoanelor din organizația dvs**. De exemplu, dacă mesajul a fost trimis la o adresă Gmail, nu vă puteți retrage memoria.
- Puteți să **rememorați doar mesajele trimise din Outlook pentru PC**. Dacă un utilizator trimite un mesaj utilizând Outlook pentru Mac sau Outlook pe web, nu vă puteți retrage memoria.
- În calitate de administrator al entității găzduite, puteți să retrageți **mesaje în numele utilizatorilor, utilizând PowerShell** (pentru mai multe informații, consultați: [căutarea și ștergerea mesajelor de e-mail](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Nu puteți retrage mesaje din centrul de administrare. Defilați în jos la "Căutați și ștergeți mesajele de e-mail din organizație" pentru mai multe informații.

**Retragerea sau înlocuirea unui mesaj de e-mail pe care l-ați trimis**

1. În panoul de foldere din partea stângă a ferestrei Outlook, alegeți folderul Elemente trimise.
2. Deschideți mesajul pe care doriți să-l rememorați. Trebuie să faceți dublu clic pentru a deschide mesajul. Selectarea mesajului astfel încât să apară în panoul de citire nu vă permite să rememorați mesajul.
3. Din fila mesaj, selectați **acțiuni**  >  **retragerea acestui mesaj**.
4. Alegeți **ștergeți copiile necitite ale acestui mesaj** sau **Ștergeți copii necitite și înlocuiți cu un mesaj nou**, apoi selectați **OK**.
5. Dacă trimiteți un mesaj de înlocuire, compuneți mesajul, apoi selectați **Trimitere**.
6. Succesul sau nereușita unui mesaj retras depinde de setările destinatarilor în Outlook.

Pentru mai multe informații, inclusiv despre cum să verificați retragerea, consultați [retragerea sau înlocuirea unui mesaj de e-mail pe care l-ați trimis](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

**_Pentru a căuta și a șterge mesaje de e-mail din organizația dvs_**., este mai ușor dacă sunteți administrator global. Dacă nu sunteți administrator global, contul trebuie adăugat la grupul de roluri eDiscovery Manager sau la rolul de gestionare a căutării conformității. Pentru a șterge mesaje, va trebui să vă asociați grupului de roluri pentru gestionarea organizației sau rolul de gestionare a căutării și eliminării. Permisiunile pentru aceste roluri sunt atribuite în [Centrul de securitate & conformitate](https://protection.office.com/).

1. [Creați o căutare de conținut](https://docs.microsoft.com/microsoft-365/compliance/content-search) pentru a găsi mesajul de șters.
2. [Conectați-vă la Security & Conformity Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Dacă utilizați Mae (multi-factor Authentication), consultați [conectarea la Microsoft 365 Security & Conformity Center PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
