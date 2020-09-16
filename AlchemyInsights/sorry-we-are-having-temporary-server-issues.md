---
title: Remedierea aplicațiilor Microsoft 365 ne pare rău, avem mesaje temporare de probleme cu serverul
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758257"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="cca79-102">Remedierea aplicațiilor Microsoft 365 "Ne pare rău, avem probleme cu serverul temporare"</span><span class="sxs-lookup"><span data-stu-id="cca79-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="cca79-103">Dacă primiți acest mesaj, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="cca79-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="cca79-104">Verificați firewallul, software-ul antivirus și setările proxy pentru a confirma că nu blochează accesul la internet la aplicațiile Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cca79-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="cca79-105">Vedeți [adresele URL și intervalele de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="cca79-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="cca79-106">Accesați **Start**  >  **Run**, apoi tastați **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="cca79-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="cca79-107">Asigurați-vă că toate următoarele servicii sunt în execuție:</span><span class="sxs-lookup"><span data-stu-id="cca79-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="cca79-108">Configurarea automată a dispozitivelor conectate la rețea</span><span class="sxs-lookup"><span data-stu-id="cca79-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="cca79-109">Serviciu listă de rețele</span><span class="sxs-lookup"><span data-stu-id="cca79-109">Network List Service</span></span>
    - <span data-ttu-id="cca79-110">Conștientizarea locației rețelei</span><span class="sxs-lookup"><span data-stu-id="cca79-110">Network Location Awareness</span></span>
    - <span data-ttu-id="cca79-111">Jurnal de evenimente Windows</span><span class="sxs-lookup"><span data-stu-id="cca79-111">Windows Event Log</span></span>

<span data-ttu-id="cca79-112">Dacă unul dintre aceste servicii nu rulează, încercați să-l porniți.</span><span class="sxs-lookup"><span data-stu-id="cca79-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="cca79-113">Dacă aveți o problemă la pornirea serviciului, derulează următoarea comandă deschizând o linie de comandă cu permisiuni ridicate:</span><span class="sxs-lookup"><span data-stu-id="cca79-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="cca79-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="cca79-114">**sfc /scannow**</span></span>

<span data-ttu-id="cca79-115">După ce se termină această comandă, reporniți computerul.</span><span class="sxs-lookup"><span data-stu-id="cca79-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="cca79-116">Pentru informații detaliate, consultați ["Ne pare rău, nu ne putem conecta la contul dvs. Vă rugăm să încercați din nou mai târziu "eroare la activare](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="cca79-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>