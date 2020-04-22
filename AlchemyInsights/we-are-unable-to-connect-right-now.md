---
title: Problemă de activare - Nu ne putem conecta chiar acum
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716184"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="b0406-102">Remedierea mesajului Office apps "Nu ne putem conecta chiar acum"</span><span class="sxs-lookup"><span data-stu-id="b0406-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="b0406-103">Dacă primiți acest mesaj, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="b0406-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="b0406-104">Verificați setările paravanului de protecție, ale software-ului antivirus și ale proxy-ului pentru a confirma că nu blochează accesul la Internet la aplicațiile Office.</span><span class="sxs-lookup"><span data-stu-id="b0406-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="b0406-105">Consultați [Adrese URL Microsoft și intervale de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="b0406-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="b0406-106">Du-te la **Scrobeală** > **A alerga**, apoi apoi tip **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="b0406-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="b0406-107">Asigurați-vă că toate serviciile se execută:</span><span class="sxs-lookup"><span data-stu-id="b0406-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="b0406-108">Configurare automată dispozitive conectate la rețea</span><span class="sxs-lookup"><span data-stu-id="b0406-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="b0406-109">Serviciu listă de rețea</span><span class="sxs-lookup"><span data-stu-id="b0406-109">Network List Service</span></span>
    - <span data-ttu-id="b0406-110">Vizibilitatea locației rețelei</span><span class="sxs-lookup"><span data-stu-id="b0406-110">Network Location Awareness</span></span>
    - <span data-ttu-id="b0406-111">Jurnal de evenimente Windows</span><span class="sxs-lookup"><span data-stu-id="b0406-111">Windows Event Log</span></span>

<span data-ttu-id="b0406-112">Dacă unul dintre aceste servicii nu funcționează, încercați să-l porniți.</span><span class="sxs-lookup"><span data-stu-id="b0406-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="b0406-113">Dacă aveți o problemă la pornirea serviciului, executați următoarea comandă deschizând un prompt de comandă cu permisiuni privilegiate:</span><span class="sxs-lookup"><span data-stu-id="b0406-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="b0406-114">**sfc /scannow sfc / scannow sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="b0406-114">**sfc /scannow**</span></span>

<span data-ttu-id="b0406-115">După ce se termină această comandă, reporniți computerul.</span><span class="sxs-lookup"><span data-stu-id="b0406-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="b0406-116">Pentru informații detaliate, consultați ["Ne pare rău, nu ne putem conecta la contul dvs. Încercați din nou mai târziu" eroare atunci când activați Office de la Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="b0406-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>