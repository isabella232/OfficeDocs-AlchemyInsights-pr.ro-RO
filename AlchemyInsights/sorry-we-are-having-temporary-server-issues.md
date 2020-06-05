---
title: Remedierea aplicațiilor Microsoft 365 Ne pare rău, avem mesaj de probleme temporare de server
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582715"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="9d40e-102">Remedierea microsoft 365 apps "Ne pare rău, avem probleme temporare server" mesaj</span><span class="sxs-lookup"><span data-stu-id="9d40e-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="9d40e-103">Dacă primiți acest mesaj, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="9d40e-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="9d40e-104">Verificați setările paravanului de protecție, ale software-ului antivirus și proxy pentru a confirma că nu blochează accesul la Internet la aplicațiile Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9d40e-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="9d40e-105">Consultați [URL-uri și intervale de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="9d40e-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="9d40e-106">Du-te la **Scrobeală**  >  **A alerga**, apoi apoi tip **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="9d40e-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="9d40e-107">Asigurați-vă că toate serviciile se execută:</span><span class="sxs-lookup"><span data-stu-id="9d40e-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="9d40e-108">Configurare automată dispozitive conectate la rețea</span><span class="sxs-lookup"><span data-stu-id="9d40e-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="9d40e-109">Serviciu listă de rețea</span><span class="sxs-lookup"><span data-stu-id="9d40e-109">Network List Service</span></span>
    - <span data-ttu-id="9d40e-110">Vizibilitatea locației rețelei</span><span class="sxs-lookup"><span data-stu-id="9d40e-110">Network Location Awareness</span></span>
    - <span data-ttu-id="9d40e-111">Jurnal de evenimente Windows</span><span class="sxs-lookup"><span data-stu-id="9d40e-111">Windows Event Log</span></span>

<span data-ttu-id="9d40e-112">Dacă unul dintre aceste servicii nu funcționează, încercați să-l porniți.</span><span class="sxs-lookup"><span data-stu-id="9d40e-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="9d40e-113">Dacă aveți o problemă la pornirea serviciului, executați următoarea comandă deschizând un prompt de comandă cu permisiuni privilegiate:</span><span class="sxs-lookup"><span data-stu-id="9d40e-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="9d40e-114">**sfc /scannow sfc / scannow sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="9d40e-114">**sfc /scannow**</span></span>

<span data-ttu-id="9d40e-115">După ce se termină această comandă, reporniți computerul.</span><span class="sxs-lookup"><span data-stu-id="9d40e-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="9d40e-116">Pentru informații detaliate, consultați ["Ne pare rău, nu ne putem conecta la contul dvs. Încercați din nou mai târziu" eroare atunci când activați](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="9d40e-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>