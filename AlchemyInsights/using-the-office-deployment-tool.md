---
title: Utilizând instrumentul de implementare Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28307398"
---
# <a name="using-the-office-deployment-tool-odt"></a>Utilizând instrumentul de implementare Office (ODT)

Utilizaţi instrumentul de implementare Office (ODT) să implementaţi Office 365 versiunile de birou. Instrumentul de implementare Office (setup.exe) este executat din linia de comandă şi utilizează un fişier de configurare XML pentru a determina ce setări să se aplice la implementarea Office.
  
1. Descărcaţi cea mai recentă versiune a instrumentului de implementare Office la [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
    
2. Utilizaţi [Instrumentul de personalizare Office (OCT)](https://config.office.com) să selectaţi preferinţele de implementare şi de a crea fişierul de configurare XML. Fişierul de configurare de export şi puneţi-l la nivel local pe acelaşi folder unde locuieşte setup.exe. 
    
    **Notă:** Instalare Office probleme apar frecvent datorate a configurat greşit sau fişiere de configurare malformatted. Pentru a evita astfel de probleme, vă recomandăm să utilizaţi instrumentul de particularizare Office pentru a crea fişierul de configurare. Asemenea, puteţi importa fişiere de configurare existente în instrumentul de personalizare Office. 
    
3. La un ascensor virgulă prompt, comutaţi la locaţia unde locuieşte setup.exe şi executaţi instrumentul de implementare Office în modul de descărcare şi specificaţi fişierul de configurare pe care tocmai aţi salvat. În acest exemplu, fişierul de configurare este denumit einkommentiert:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Executaţi instrumentul de implementare Office în modul de configurare şi specificaţi fişierul de configurare.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Notă:** Trebuie să executaţi acest pas la computerul client pe care doriţi să instalaţi Office şi trebuie să aveţi permisiuni de local administrator pe acel computer. 
    
Pentru a afla mai multe despre utilizarea instrumentului de implementare Office pentru dumneavoastră Office 365 ProPlus scenarii de implementare, consultaţi [Prezentare generală a instrumentului de implementare Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Pentru mai multe detalii despre cum se utilizează instrumentul de particularizare Office, consultaţi [Prezentare generală a instrumentului de personalizare Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

