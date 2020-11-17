---
title: Utilizarea instrumentului de implementare Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085844"
---
# <a name="using-the-office-deployment-tool-odt"></a>Utilizarea instrumentului de implementare Office (ODT)

Utilizați instrumentul de implementare Office (ODT) pentru a implementa versiunile Office 365 de Office. Instrumentul de implementare Office (setupodt.exe) este rulat din linia de comandă și utilizează un fișier XML de configurare pentru a determina ce setări să se aplice atunci când implementați Office.
  
1. Descărcați cea mai recentă versiune a instrumentului de implementare Office de la [Centrul de descărcare Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Utilizați [Instrumentul de particularizare Office (Oct)](https://config.office.com) pentru a selecta preferințele de implementare și a crea fișierul XML de configurare. Exportați fișierul de configurare și amplasați-l local în același folder în care se află setupodt.exe.

    **Notă:** Problemele de instalare Office apar frecvent din cauza fișierelor de configurare incorect configurate sau malformatted. Pentru a evita astfel de probleme, vă recomandăm să utilizați instrumentul de particularizare Office pentru a crea fișierul de configurare. De asemenea, puteți importa fișiere de configurare existente în instrumentul de particularizare Office.

3. Dintr-o linie de comandă privilegiat, comutați la locația unde setupodt.exe se află și rulați instrumentul de implementare Office în modul de descărcare și specificați fișierul de configurare pe care tocmai l-ați salvat. În acest exemplu, fișierul de configurare este denumit Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. Rulați instrumentul de implementare Office în modul de configurare și specificați fișierul de configurare.

```setupodt.exe /configure Configuration.xml```

**Notă:** Trebuie să parcurgeți acest pas de pe computerul client pe care doriți să instalați Office și trebuie să aveți permisiuni de administrator local pe acel computer.

Pentru a afla mai multe despre utilizarea instrumentului de implementare Office pentru scenariile de implementare Microsoft 365 pentru aplicațiile Enterprise, consultați [prezentarea generală a instrumentului de implementare Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Pentru mai multe detalii despre cum să utilizați instrumentul de particularizare Office, consultați [prezentarea generală a instrumentului de particularizare Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
