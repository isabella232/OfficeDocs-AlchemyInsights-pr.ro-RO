---
title: Utilizarea Instrumentului Office implementare sistem
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083782"
---
# <a name="using-the-office-deployment-tool-odt"></a>Utilizarea instrumentului Office de implementare pentru text (ODT)

Utilizați Instrumentul de implementare Office (ODT) pentru a implementa Office 365 de Office. Instrumentul Office de implementare (setup.exe) rulează din linia de comandă și utilizează un fișier XML de configurare pentru a determina ce setări să se aplice atunci când implementați Office.
  
1. Descărcați cea mai recentă versiune a Office de implementare din [Centrul de descărcare Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Utilizați instrumentul [de Office pentru a selecta preferințele](https://config.office.com) de implementare și a crea fișierul XML de configurare. Exportați fișierul de configurare și plasați-l local în același folder în care se setup.exe dvs.

    **Notă:** Office de instalare apar de obicei din cauza fișierelor de configurare configurate greșit sau cu malformatare. Pentru a evita astfel de probleme, vă recomandăm să utilizați instrumentul Office de particularizare pentru a crea fișierul de configurare. De asemenea, puteți importa fișierele de configurare existente în Office de particularizare.

3. Dintr-o linie de comandă cu nivel ridicat, comutați la locația în care se află setup.exe și rulați Instrumentul de implementare Office în modul de descărcare și specificați fișierul de configurare pe care tocmai l-ați salvat. În acest exemplu, fișierul de configurare se numește Configuration.xml:

```setup.exe /download Configuration.xml```

4.Rulați instrumentul Office de implementare în modul de configurare și specificați fișierul de configurare.

```setup.exe /configure Configuration.xml```

**Notă:** Trebuie să rulați acest pas de pe computerul client pe care doriți să instalați Office și trebuie să aveți permisiuni de administrator local pe acel computer.

Pentru a afla mai multe despre utilizarea Instrumentului de implementare Office pentru scenariile Aplicații Microsoft 365 pentru întreprindere implementare, consultați Prezentare generală a [Instrumentului de implementare Office.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Pentru mai multe detalii despre utilizarea Instrumentului de Office, consultați Prezentare generală a [Instrumentului Office particularizare.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
