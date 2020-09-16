---
title: Problemă de activare-nu ne putem conecta acum
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725995"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="4e25c-102">Remedierea aplicațiilor Microsoft 365 "nu ne putem conecta acum"</span><span class="sxs-lookup"><span data-stu-id="4e25c-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="4e25c-103">Dacă primiți acest mesaj, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="4e25c-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="4e25c-104">Verificați firewallul, software-ul antivirus și setările proxy pentru a confirma că nu blochează accesul la internet la aplicațiile Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4e25c-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="4e25c-105">Vedeți [adresele URL și intervalele de adrese IP Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="4e25c-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="4e25c-106">Accesați **Start**  >  **Run**, apoi tastați **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="4e25c-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="4e25c-107">Asigurați-vă că toate următoarele servicii sunt în execuție:</span><span class="sxs-lookup"><span data-stu-id="4e25c-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="4e25c-108">Configurarea automată a dispozitivelor conectate la rețea</span><span class="sxs-lookup"><span data-stu-id="4e25c-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="4e25c-109">Serviciu listă de rețele</span><span class="sxs-lookup"><span data-stu-id="4e25c-109">Network List Service</span></span>
    - <span data-ttu-id="4e25c-110">Conștientizarea locației rețelei</span><span class="sxs-lookup"><span data-stu-id="4e25c-110">Network Location Awareness</span></span>
    - <span data-ttu-id="4e25c-111">Jurnal de evenimente Windows</span><span class="sxs-lookup"><span data-stu-id="4e25c-111">Windows Event Log</span></span>

<span data-ttu-id="4e25c-112">Dacă unul dintre aceste servicii nu rulează, încercați să-l porniți.</span><span class="sxs-lookup"><span data-stu-id="4e25c-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="4e25c-113">Dacă aveți o problemă la pornirea serviciului, derulează următoarea comandă deschizând o linie de comandă cu permisiuni ridicate:</span><span class="sxs-lookup"><span data-stu-id="4e25c-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="4e25c-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="4e25c-114">**sfc /scannow**</span></span>

<span data-ttu-id="4e25c-115">După ce se termină această comandă, reporniți computerul.</span><span class="sxs-lookup"><span data-stu-id="4e25c-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="4e25c-116">Pentru informații detaliate, consultați ["Ne pare rău, nu ne putem conecta la contul dvs. Vă rugăm să încercați din nou mai târziu "eroare atunci când activați Office de la Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="4e25c-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>