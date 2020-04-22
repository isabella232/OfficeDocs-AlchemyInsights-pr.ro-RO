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
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726260"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="a89ab-102">Utilizarea instrumentului de implementare Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="a89ab-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="a89ab-103">Utilizați Instrumentul de implementare Office (ODT) pentru a implementa versiunile Office 365 office.</span><span class="sxs-lookup"><span data-stu-id="a89ab-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="a89ab-104">Instrumentul de implementare Office (setup.exe) se execută din linia de comandă și utilizează un fișier XML de configurare pentru a determina ce setări să se aplice la implementarea Office.</span><span class="sxs-lookup"><span data-stu-id="a89ab-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="a89ab-105">Descărcați cea mai recentă versiune a Instrumentului de implementare Office de la [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="a89ab-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="a89ab-106">Utilizați [Instrumentul de particularizare Office (OCT) pentru](https://config.office.com) a selecta preferințele de implementare și a crea fișierul XML de configurare.</span><span class="sxs-lookup"><span data-stu-id="a89ab-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="a89ab-107">Exportați fișierul de configurare și plasați-l local în același folder în care se află setup.exe.</span><span class="sxs-lookup"><span data-stu-id="a89ab-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="a89ab-108">**Notã:** Probleme de instalare Office apar frecvent din cauza fișierelor de configurare configurate greșit sau malformatate.</span><span class="sxs-lookup"><span data-stu-id="a89ab-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="a89ab-109">Pentru a evita astfel de probleme, vă recomandăm să utilizați Instrumentul de particularizare Office pentru a crea fișierul de configurare.</span><span class="sxs-lookup"><span data-stu-id="a89ab-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="a89ab-110">De asemenea, aveți posibilitatea să importați fișierele de configurare existente în instrumentul de particularizare Office.</span><span class="sxs-lookup"><span data-stu-id="a89ab-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="a89ab-111">Dintr-un prompt de comandă privilegiat, comutați la locația în care se află setup.exe și executați Instrumentul de implementare Office în modul de descărcare și specificați fișierul de configurare pe care tocmai l-ați salvat.</span><span class="sxs-lookup"><span data-stu-id="a89ab-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="a89ab-112">În acest exemplu, fișierul de configurare este numit Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="a89ab-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="a89ab-113">Executați instrumentul de implementare Office în modul de configurare și specificați fișierul de configurare.</span><span class="sxs-lookup"><span data-stu-id="a89ab-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="a89ab-114">**Notã:** Trebuie să executați acest pas de pe computerul client pe care doriți să instalați Office și trebuie să aveți permisiuni de administrator local pe acel computer.</span><span class="sxs-lookup"><span data-stu-id="a89ab-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="a89ab-115">Pentru a afla mai multe despre utilizarea Instrumentului de implementare Office pentru scenariile de implementare Microsoft 365 Apps for enterprise, consultați [Prezentare generală a instrumentului de implementare Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="a89ab-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="a89ab-116">Pentru mai multe detalii despre se utilizează Instrumentul de particularizare Office, consultați [Prezentare generală a instrumentului de particularizare Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="a89ab-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
