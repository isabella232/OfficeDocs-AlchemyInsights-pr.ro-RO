---
title: Probleme la conectarea la aplicațiile Microsoft 365
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
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833051"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="32430-102">Ecran de conectare necompletat în aplicațiile Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="32430-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="32430-103">Pentru a remedia această problemă, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="32430-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="32430-104">Instalați cele mai recente actualizări [pentru Windows](https://support.microsoft.com/help/4027667/windows-10-update) și [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="32430-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="32430-105">Resetați opțiunile Internet Explorer: Accesați Instrumente Opțiuni internet - Setări complexe  >    >    >  **de resetare Internet Explorer** (rețineți că veți pierde setările particularizate), apoi încercați din nou să vă conectați la Office.</span><span class="sxs-lookup"><span data-stu-id="32430-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="32430-106">Dezactivați Windows Defender Application Guard (WDAG) sau orice program similar de firewall sau antivirus:</span><span class="sxs-lookup"><span data-stu-id="32430-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="32430-107">În Panoul de control, accesați **Programe**, apoi alegeți **Activare sau dezactivare caracteristici Windows**.</span><span class="sxs-lookup"><span data-stu-id="32430-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="32430-108">Dacă Windows Defender Application Guard este activat, încercați să-l dezactivare.</span><span class="sxs-lookup"><span data-stu-id="32430-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="32430-109">**Notă:** Poate fi necesar să reporniți computerul.</span><span class="sxs-lookup"><span data-stu-id="32430-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="32430-110">Asigurați-vă că insertul Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nu este blocat de nicio aplicație sau de program antivirus/firewall.</span><span class="sxs-lookup"><span data-stu-id="32430-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="32430-111">[Goliți acreditările Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Managerul de acreditări Windows.</span><span class="sxs-lookup"><span data-stu-id="32430-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="32430-112">**Notă:** Căile de registry pentru Office 2016 s-au modificat la 16.0.</span><span class="sxs-lookup"><span data-stu-id="32430-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="32430-113">(De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="32430-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="32430-114">Pentru mai multe informații, consultați Probleme de conectare la conectare după actualizarea la [Office 2016, compilarea 16.0.7967 din Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="32430-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>