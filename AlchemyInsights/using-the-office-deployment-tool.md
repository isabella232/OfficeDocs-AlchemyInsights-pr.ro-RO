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
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="3e37c-102">Utilizând instrumentul de implementare Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="3e37c-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="3e37c-p101">Utilizaţi instrumentul de implementare Office (ODT) să implementaţi Office 365 versiunile de birou. Instrumentul de implementare Office (setup.exe) este executat din linia de comandă şi utilizează un fişier de configurare XML pentru a determina ce setări să se aplice la implementarea Office.</span><span class="sxs-lookup"><span data-stu-id="3e37c-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="3e37c-105">Descărcaţi cea mai recentă versiune a instrumentului de implementare Office la [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="3e37c-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="3e37c-p102">Utilizaţi [Instrumentul de personalizare Office (OCT)](https://config.office.com) să selectaţi preferinţele de implementare şi de a crea fişierul de configurare XML. Fişierul de configurare de export şi puneţi-l la nivel local pe acelaşi folder unde locuieşte setup.exe.</span><span class="sxs-lookup"><span data-stu-id="3e37c-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="3e37c-p103">**Notă:** Instalare Office probleme apar frecvent datorate a configurat greşit sau fişiere de configurare malformatted. Pentru a evita astfel de probleme, vă recomandăm să utilizaţi instrumentul de particularizare Office pentru a crea fişierul de configurare. Asemenea, puteţi importa fişiere de configurare existente în instrumentul de personalizare Office.</span><span class="sxs-lookup"><span data-stu-id="3e37c-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="3e37c-p104">La un ascensor virgulă prompt, comutaţi la locaţia unde locuieşte setup.exe şi executaţi instrumentul de implementare Office în modul de descărcare şi specificaţi fişierul de configurare pe care tocmai aţi salvat. În acest exemplu, fişierul de configurare este denumit einkommentiert:</span><span class="sxs-lookup"><span data-stu-id="3e37c-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="3e37c-113">Executaţi instrumentul de implementare Office în modul de configurare şi specificaţi fişierul de configurare.</span><span class="sxs-lookup"><span data-stu-id="3e37c-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="3e37c-114">**Notă:** Trebuie să executaţi acest pas la computerul client pe care doriţi să instalaţi Office şi trebuie să aveţi permisiuni de local administrator pe acel computer.</span><span class="sxs-lookup"><span data-stu-id="3e37c-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="3e37c-p105">Pentru a afla mai multe despre utilizarea instrumentului de implementare Office pentru dumneavoastră Office 365 ProPlus scenarii de implementare, consultaţi [Prezentare generală a instrumentului de implementare Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Pentru mai multe detalii despre cum se utilizează instrumentul de particularizare Office, consultaţi [Prezentare generală a instrumentului de personalizare Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="3e37c-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

