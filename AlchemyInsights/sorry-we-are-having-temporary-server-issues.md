---
title: Remedierea aplicațiilor Office Ne pare rău, avem mesaj de probleme temporare de server
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764129"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="0d108-102">Remedierea office apps "Ne pare rău, avem probleme temporare server" mesaj</span><span class="sxs-lookup"><span data-stu-id="0d108-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="0d108-103">Dacă primiți acest mesaj, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="0d108-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="0d108-104">Verificați setările paravanului de protecție, ale software-ului antivirus și ale proxy-ului pentru a confirma că nu blochează accesul la Internet la aplicațiile Office.</span><span class="sxs-lookup"><span data-stu-id="0d108-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="0d108-105">Consultați [URL-uri și intervale de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="0d108-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="0d108-106">Du-te la **Scrobeală** > **A alerga**, apoi apoi tip **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="0d108-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="0d108-107">Asigurați-vă că toate serviciile se execută:</span><span class="sxs-lookup"><span data-stu-id="0d108-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="0d108-108">Configurare automată dispozitive conectate la rețea</span><span class="sxs-lookup"><span data-stu-id="0d108-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="0d108-109">Serviciu listă de rețea</span><span class="sxs-lookup"><span data-stu-id="0d108-109">Network List Service</span></span>
    - <span data-ttu-id="0d108-110">Vizibilitatea locației rețelei</span><span class="sxs-lookup"><span data-stu-id="0d108-110">Network Location Awareness</span></span>
    - <span data-ttu-id="0d108-111">Jurnal de evenimente Windows</span><span class="sxs-lookup"><span data-stu-id="0d108-111">Windows Event Log</span></span>

<span data-ttu-id="0d108-112">Dacă unul dintre aceste servicii nu funcționează, încercați să-l porniți.</span><span class="sxs-lookup"><span data-stu-id="0d108-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="0d108-113">Dacă aveți o problemă la pornirea serviciului, executați următoarea comandă deschizând un prompt de comandă cu permisiuni privilegiate:</span><span class="sxs-lookup"><span data-stu-id="0d108-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="0d108-114">**sfc /scannow sfc / scannow sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="0d108-114">**sfc /scannow**</span></span>

<span data-ttu-id="0d108-115">După ce se termină această comandă, reporniți computerul.</span><span class="sxs-lookup"><span data-stu-id="0d108-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="0d108-116">Pentru informații detaliate, consultați ["Ne pare rău, nu ne putem conecta la contul dvs. Încercați din nou mai târziu" eroare atunci când activați](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="0d108-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>