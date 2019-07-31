---
title: Probleme de sign in la Office apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938311"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="e6899-102">Semn-înăuntru ecran gol în Office apps</span><span class="sxs-lookup"><span data-stu-id="e6899-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="e6899-103">Pentru a remedia această problemă, încercaţi următoarele:</span><span class="sxs-lookup"><span data-stu-id="e6899-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="e6899-104">Instalaţi cele mai recente actualizări pentru [Windows](https://support.microsoft.com/help/4027667/windows-10-update) si [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="e6899-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="e6899-105">Reiniţializaţi Internet Explorer opţiuni: Du-te la **Instrumente** > **Opţiuni Internet** > **Advanced** > **Reinițializare setări Internet Explorer** (Notă de faptul că veţi pierde setările particularizate), şi apoi încercaţi conectarea la biroul din nou.</span><span class="sxs-lookup"><span data-stu-id="e6899-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="e6899-106">Dezactivează Windows Defender cerere Garda (WDAG) sau orice program firewall sau anti-virus similar:</span><span class="sxs-lookup"><span data-stu-id="e6899-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="e6899-107">În panoul de Control, du-te la **programe**, şi apoi alegeţi **Nap Ferestre features on sau off**.</span><span class="sxs-lookup"><span data-stu-id="e6899-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="e6899-108">În cazul în care Garda de aplicaţie Windows Defender este activat, încercaţi să dezactivaţi-l.</span><span class="sxs-lookup"><span data-stu-id="e6899-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="e6899-109">**Notă:** Trebuie să reporniţi computerul.</span><span class="sxs-lookup"><span data-stu-id="e6899-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="e6899-110">Asiguraţi-vă că Microsoft.AAD.BrokerPlugin [Dai WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nu este blocat de vreo aplicaţie sau un program firewall/anti-anti-virus.</span><span class="sxs-lookup"><span data-stu-id="e6899-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="e6899-111">[Acreditări clar Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="e6899-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="e6899-112">**Notă:** Căi de registry pentru Office 2016 s-au schimbat la 16,0.</span><span class="sxs-lookup"><span data-stu-id="e6899-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e6899-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="e6899-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="e6899-114">Pentru informaţii suplimentare, consultaţi [probleme de conexiune în semn-înăuntru după update la Office 2016 construi 16.0.7967 pe Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="e6899-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>