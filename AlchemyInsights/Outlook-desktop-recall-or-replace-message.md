---
title: Outlook Retragerea sau înlocuirea unui mesaj de e-mail pe desktop
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
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918407"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Retragerea sau înlocuirea unui mesaj de Outlook e-mail

- Ca administrator, puteți retragerea **mesajelor în numele utilizatorilor care utilizează PowerShell.** Nu puteți retragerea mesajelor din centrul de administrare.
- Puteți retragerea **doar a mesajelor care sunt trimise persoanelor din organizația dvs.** Dacă mesajul a fost trimis la o adresă Gmail, de exemplu, nu-l puteți aminti.
- Puteți retragerea **mesajelor trimise doar de Outlook 2016 de pe PC.** Dacă un utilizator trimite un mesaj utilizând Outlook pentru Mac sau Outlook pe web, nu îl puteți reaminti.

Pentru a retragerea sau înlocuirea unui mesaj de e-mail:

1. În panoul de foldere din partea stângă a ferestrei Outlook, selectați folderul Elemente trimise.
1. Faceți dublu clic pe mesajul pe care doriți să-l retrasți pentru a-l deschide.
1. Selectați **fila Mesaj,** apoi selectați **Acțiuni** Retragerea  >  **acestui mesaj**.
1. Selectați **Ștergeți copii necitite ale acestui mesaj sau** **Ștergerea copiilor necitite** și înlocuirea cu un mesaj nou , apoi selectați **OK**.
1. Dacă trimiteți un mesaj de înlocuire, compuneți mesajul, apoi selectați **Trimitere**.
1. Reușita sau eșecul retragerea unui mesaj depinde de setările destinatarului din Outlook. Pentru pașii necesari verificării retragerea, consultați [acest articol.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Căutarea și ștergerea mesajelor de e-mail din organizația dvs.

- Dacă nu sunt administrator global, contul dvs. trebuie să fie adăugat la rolul Manager pentru descoperirea informațiilor electronic sau la rolul de gestionare a căutării de conformitate pentru a căuta mesaje. Pentru a șterge mesaje, va trebui să vă asociați grupului de roluri Gestionare organizație sau rolului de gestionare a căutării și ștergerii definitiv. Permisiunile pentru aceste roluri sunt atribuite în Centrul [de securitate și conformitate.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Creați o căutare de conținut](https://docs.microsoft.com/microsoft-365/compliance/content-search) pentru a găsi mesajul de șters.
- [Conectare powerShell către Centrul de securitate și conformitate.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Dacă utilizați Multi-Factor Authentication, consultați autentificarea prin mai Conectare pentru a Microsoft 365 PowerShell utilizând [Multi-Factor Authentication.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)