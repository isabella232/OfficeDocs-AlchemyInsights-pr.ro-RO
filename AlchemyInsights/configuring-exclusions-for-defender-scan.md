---
title: Configurarea excluderilor pentru Microsoft Defender ATP Scan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713903"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="df993-102">Configurarea excluderilor pentru Microsoft Defender ATP Scan</span><span class="sxs-lookup"><span data-stu-id="df993-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="df993-103">În general, puteți să excludeți anumite extensii de fișier și locații de foldere din scanările ATP Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="df993-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="df993-104">De asemenea, puteți configura excluderi pentru fișierele deschise de anumite procese.</span><span class="sxs-lookup"><span data-stu-id="df993-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="df993-105">Pentru mai multe informații, consultați [Configurarea și validarea excluderilor pe baza extensiei de fișier și a locației folderului](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) și [Configurarea excluderilor pentru fișierele deschise de procese](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="df993-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="df993-106">Pentru a configura excluderi pentru  **Windows server 2016 și 2019**, consultați [Configurarea excluderilor antivirus Microsoft Defender pe Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="df993-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="df993-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="df993-107">**Mac**</span></span>

<span data-ttu-id="df993-108">Pentru detalii despre tipurile de excluderi acceptate și configurarea unei liste de excluderi pentru Mac, consultați [tipuri de excluderi acceptate](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) și [cum să configurați lista de excluderi](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="df993-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="df993-109">**Notă** De asemenea, puteți să validați listele de excluderi utilizând fișierul de test EICAR.</span><span class="sxs-lookup"><span data-stu-id="df993-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="df993-110">Pentru mai multe informații, consultați [validarea listelor de excluderi cu fișierul de test EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="df993-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="df993-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="df993-111">**Linux**</span></span>

<span data-ttu-id="df993-112">Pentru detalii despre tipurile de excluderi acceptate și configurarea unei liste de excluderi pentru Linux, consultați [tipuri de excluderi acceptate](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) și [Configurarea și validarea excluderilor pentru Microsoft Defender ATP pentru Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="df993-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="df993-113">**Notă** De asemenea, puteți să validați listele de excluderi utilizând fișierul de test EICAR.</span><span class="sxs-lookup"><span data-stu-id="df993-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="df993-114">Pentru mai multe informații, consultați [validarea listelor de excluderi cu fișierul de test EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="df993-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 