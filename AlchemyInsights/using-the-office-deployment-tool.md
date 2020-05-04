---
title: Utilizarea instrumentului de implementare Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010879"
---
# <a name="using-the-office-deployment-tool-odt"></a>Utilizarea instrumentului de implementare Office (ODT)

Utilizați Instrumentul de implementare Office (ODT) pentru a implementa versiunile Office 365 office. Instrumentul de implementare Office (setup.exe) se execută din linia de comandă și utilizează un fișier XML de configurare pentru a determina ce setări să se aplice la implementarea Office.
  
1. Descărcați cea mai recentă versiune a Instrumentului de implementare Office de la [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Utilizați [Instrumentul de particularizare Office (OCT) pentru](https://config.office.com) a selecta preferințele de implementare și a crea fișierul XML de configurare. Exportați fișierul de configurare și plasați-l local în același folder în care se află setup.exe.

    **Notã:** Probleme de instalare Office apar frecvent din cauza fișierelor de configurare configurate greșit sau malformatate. Pentru a evita astfel de probleme, vă recomandăm să utilizați Instrumentul de particularizare Office pentru a crea fișierul de configurare. De asemenea, aveți posibilitatea să importați fișierele de configurare existente în instrumentul de particularizare Office.

3. Dintr-un prompt de comandă privilegiat, comutați la locația în care se află setup.exe și executați Instrumentul de implementare Office în modul de descărcare și specificați fișierul de configurare pe care tocmai l-ați salvat. În acest exemplu, fișierul de configurare este numit Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Executați instrumentul de implementare Office în modul de configurare și specificați fișierul de configurare.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Notã:** Trebuie să executați acest pas de pe computerul client pe care doriți să instalați Office și trebuie să aveți permisiuni de administrator local pe acel computer.

Pentru a afla mai multe despre utilizarea Instrumentului de implementare Office pentru scenariile de implementare Microsoft 365 Apps for enterprise, consultați [Prezentare generală a instrumentului de implementare Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Pentru mai multe detalii despre se utilizează Instrumentul de particularizare Office, consultați [Prezentare generală a instrumentului de particularizare Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
