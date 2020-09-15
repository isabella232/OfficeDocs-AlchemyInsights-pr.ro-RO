---
title: Probleme la conectarea la aplicațiile Microsoft 365
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
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695299"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="b9eb4-102">Ecran de conectare necompletat în aplicațiile Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b9eb4-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="b9eb4-103">Pentru a remedia această problemă, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="b9eb4-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="b9eb4-104">Instalați cele mai recente actualizări pentru [Windows](https://support.microsoft.com/help/4027667/windows-10-update) și [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="b9eb4-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="b9eb4-105">Reinițializarea opțiunilor Internet Explorer: accesați **Instrumente**  >  **Opțiuni Internet**  >  **Advanced**  >  **reinițializați setările Internet Explorer** (rețineți că veți pierde setările particularizate), apoi încercați din nou să vă conectați la Office.</span><span class="sxs-lookup"><span data-stu-id="b9eb4-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="b9eb4-106">Dezactivați Garda de aplicații Windows Defender (WDAG) sau orice alt program de firewall sau antivirus similar:</span><span class="sxs-lookup"><span data-stu-id="b9eb4-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="b9eb4-107">În panoul de control, accesați **programe**, apoi alegeți **Activare sau dezactivare caracteristici Windows**.</span><span class="sxs-lookup"><span data-stu-id="b9eb4-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="b9eb4-108">Dacă Garda de aplicație Windows Defender este activată, încercați să o dezactivați.</span><span class="sxs-lookup"><span data-stu-id="b9eb4-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="b9eb4-109">**Notă:** Poate fi necesar să reporniți computerul.</span><span class="sxs-lookup"><span data-stu-id="b9eb4-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="b9eb4-110">Asigurați-vă că [insertul](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. aad. BROKERPLUGIN Dan WAM nu este blocat de nicio aplicație sau de un program firewall/antivirus.</span><span class="sxs-lookup"><span data-stu-id="b9eb4-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="b9eb4-111">[Debifați acreditările Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând managerul de acreditări Windows.</span><span class="sxs-lookup"><span data-stu-id="b9eb4-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="b9eb4-112">**Notă:** Căile de registry pentru Office 2016 s-au modificat la 16,0.</span><span class="sxs-lookup"><span data-stu-id="b9eb4-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b9eb4-113">(De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="b9eb4-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="b9eb4-114">Pentru mai multe informații, consultați [probleme de conexiune în conectarea după actualizare la Office 2016 Build 16.0.7967 pe Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="b9eb4-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>