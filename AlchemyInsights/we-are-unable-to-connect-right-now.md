---
title: Problemă de activare - Nu vă putem conecta momentan
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806454"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="9062c-102">Remedierea aplicațiilor Microsoft 365 Mesajul "Nu vă putem conecta momentan"</span><span class="sxs-lookup"><span data-stu-id="9062c-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="9062c-103">Dacă primiți acest mesaj, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="9062c-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="9062c-104">Verificați setările pentru firewall, software antivirus și proxy pentru a confirma că nu blochează accesul la internet la aplicațiile Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9062c-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="9062c-105">Consultați [Adrese URL și intervale de adrese IP Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="9062c-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="9062c-106">Accesați **Start**  >  **Run**, apoi tastați **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="9062c-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="9062c-107">Asigurați-vă că toate serviciile următoare rulează:</span><span class="sxs-lookup"><span data-stu-id="9062c-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="9062c-108">Configurarea automată a dispozitivelor conectate la rețea</span><span class="sxs-lookup"><span data-stu-id="9062c-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="9062c-109">Serviciul Listă de rețea</span><span class="sxs-lookup"><span data-stu-id="9062c-109">Network List Service</span></span>
    - <span data-ttu-id="9062c-110">Informații despre locația de rețea</span><span class="sxs-lookup"><span data-stu-id="9062c-110">Network Location Awareness</span></span>
    - <span data-ttu-id="9062c-111">Jurnal de evenimente Windows</span><span class="sxs-lookup"><span data-stu-id="9062c-111">Windows Event Log</span></span>

<span data-ttu-id="9062c-112">Dacă unul dintre aceste servicii nu rulează, încercați să îl porniți.</span><span class="sxs-lookup"><span data-stu-id="9062c-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="9062c-113">Dacă aveți o problemă la pornirea serviciului, rulați următoarea comandă deschizând o linie de comandă cu permisiuni cu drepturi înălțimii:</span><span class="sxs-lookup"><span data-stu-id="9062c-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="9062c-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="9062c-114">**sfc /scannow**</span></span>

<span data-ttu-id="9062c-115">După ce se termină această comandă, reporniți computerul.</span><span class="sxs-lookup"><span data-stu-id="9062c-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="9062c-116">Pentru informații detaliate, [consultați "Ne pare rău, nu ne putem conecta la contul dvs. Încercați din nou mai târziu" atunci când activați Office din Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="9062c-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>