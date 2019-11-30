---
title: Fixarea aplicațiilor Office ne pare rău, avem un mesaj temporar probleme de server
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628002"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="bd601-102">Fixarea aplicațiilor Office "Ne pare rău, avem probleme temporare de server" mesaj</span><span class="sxs-lookup"><span data-stu-id="bd601-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="bd601-103">Dacă primiți acest mesaj, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="bd601-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="bd601-104">Verificați Paravanul de protecție, software-ul antivirus și setările proxy pentru a confirma că acestea nu blochează accesul la internet la aplicațiile Office.</span><span class="sxs-lookup"><span data-stu-id="bd601-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="bd601-105">Consultați [Office 365 URL-uri și intervale de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="bd601-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="bd601-106">Du-te la **scrobeală** > a**alerga**, și apoi atunci tip **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="bd601-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="bd601-107">Asigurați-vă că următoarele servicii se execută toate:</span><span class="sxs-lookup"><span data-stu-id="bd601-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="bd601-108">Instalare automată dispozitive conectate la rețea</span><span class="sxs-lookup"><span data-stu-id="bd601-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="bd601-109">Serviciu listă de rețea</span><span class="sxs-lookup"><span data-stu-id="bd601-109">Network List Service</span></span>
    - <span data-ttu-id="bd601-110">Vizibilitate Locație rețea</span><span class="sxs-lookup"><span data-stu-id="bd601-110">Network Location Awareness</span></span>
    - <span data-ttu-id="bd601-111">Jurnal de evenimente Windows</span><span class="sxs-lookup"><span data-stu-id="bd601-111">Windows Event Log</span></span>

<span data-ttu-id="bd601-112">Dacă unul dintre aceste servicii nu se execută, încercați să-l porniți.</span><span class="sxs-lookup"><span data-stu-id="bd601-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="bd601-113">Dacă aveți o problemă la pornirea serviciului, executați următoarea comandă deschizând un prompt de comandă cu permisiuni elevate:</span><span class="sxs-lookup"><span data-stu-id="bd601-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="bd601-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="bd601-114">**sfc /scannow**</span></span>

<span data-ttu-id="bd601-115">După terminarea acestei comenzi, reporniți computerul.</span><span class="sxs-lookup"><span data-stu-id="bd601-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="bd601-116">Pentru informații detaliate, consultați ["Ne pare rău, nu ne putem conecta la contul dvs. Încercați din nou mai târziu "eroare atunci când activați Office din Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="bd601-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>