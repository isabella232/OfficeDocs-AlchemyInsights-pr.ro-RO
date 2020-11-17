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
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="6a913-102">Utilizarea instrumentului de implementare Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="6a913-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="6a913-103">Utilizați instrumentul de implementare Office (ODT) pentru a implementa versiunile Office 365 de Office.</span><span class="sxs-lookup"><span data-stu-id="6a913-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="6a913-104">Instrumentul de implementare Office (setupodt.exe) este rulat din linia de comandă și utilizează un fișier XML de configurare pentru a determina ce setări să se aplice atunci când implementați Office.</span><span class="sxs-lookup"><span data-stu-id="6a913-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="6a913-105">Descărcați cea mai recentă versiune a instrumentului de implementare Office de la [Centrul de descărcare Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="6a913-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="6a913-106">Utilizați [Instrumentul de particularizare Office (Oct)](https://config.office.com) pentru a selecta preferințele de implementare și a crea fișierul XML de configurare.</span><span class="sxs-lookup"><span data-stu-id="6a913-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="6a913-107">Exportați fișierul de configurare și amplasați-l local în același folder în care se află setupodt.exe.</span><span class="sxs-lookup"><span data-stu-id="6a913-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="6a913-108">**Notă:** Problemele de instalare Office apar frecvent din cauza fișierelor de configurare incorect configurate sau malformatted.</span><span class="sxs-lookup"><span data-stu-id="6a913-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="6a913-109">Pentru a evita astfel de probleme, vă recomandăm să utilizați instrumentul de particularizare Office pentru a crea fișierul de configurare.</span><span class="sxs-lookup"><span data-stu-id="6a913-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="6a913-110">De asemenea, puteți importa fișiere de configurare existente în instrumentul de particularizare Office.</span><span class="sxs-lookup"><span data-stu-id="6a913-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="6a913-111">Dintr-o linie de comandă privilegiat, comutați la locația unde setupodt.exe se află și rulați instrumentul de implementare Office în modul de descărcare și specificați fișierul de configurare pe care tocmai l-ați salvat.</span><span class="sxs-lookup"><span data-stu-id="6a913-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="6a913-112">În acest exemplu, fișierul de configurare este denumit Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="6a913-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="6a913-113">4. Rulați instrumentul de implementare Office în modul de configurare și specificați fișierul de configurare.</span><span class="sxs-lookup"><span data-stu-id="6a913-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="6a913-114">**Notă:** Trebuie să parcurgeți acest pas de pe computerul client pe care doriți să instalați Office și trebuie să aveți permisiuni de administrator local pe acel computer.</span><span class="sxs-lookup"><span data-stu-id="6a913-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="6a913-115">Pentru a afla mai multe despre utilizarea instrumentului de implementare Office pentru scenariile de implementare Microsoft 365 pentru aplicațiile Enterprise, consultați [prezentarea generală a instrumentului de implementare Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="6a913-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="6a913-116">Pentru mai multe detalii despre cum să utilizați instrumentul de particularizare Office, consultați [prezentarea generală a instrumentului de particularizare Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="6a913-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
