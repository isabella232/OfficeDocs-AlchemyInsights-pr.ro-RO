---
title: Instrumentul de diagnosticare a serviciului pentru Desktop virtual Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595862"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="78de2-102">Instrumentul de diagnosticare a serviciului pentru Desktop virtual Windows</span><span class="sxs-lookup"><span data-stu-id="78de2-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="78de2-103">Windows Virtual Desktop (WVD) oferă un instrument de diagnosticare care permite administratorilor să identifice erorile printr-o singură interfață.</span><span class="sxs-lookup"><span data-stu-id="78de2-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="78de2-104">Acest instrument înregistrează informații legate de diagnosticare oricând WVD este utilizat de cineva cu un rol WVD.</span><span class="sxs-lookup"><span data-stu-id="78de2-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="78de2-105">Fiecare jurnal conține informații despre rolul WVD implicat în activitate, mesajele de eroare care apar în timpul sesiunii și informațiile despre entitatea găzduită și utilizator.</span><span class="sxs-lookup"><span data-stu-id="78de2-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="78de2-106">Azure Log Analytics poate fi configurat pentru a captura jurnalul de activitate creat de instrumentul de diagnosticare urmând acești pași:</span><span class="sxs-lookup"><span data-stu-id="78de2-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="78de2-107">Creați un spațiu de lucru Analiză jurnal cu [portalul Azure](https://go.microsoft.com/fwlink/?linkid=2129500) sau [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="78de2-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="78de2-108">[Conectați computerele Windows la Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="78de2-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="78de2-109">Obțineți ID-ul spațiului de lucru și Cheia primară a spațiului de lucru.</span><span class="sxs-lookup"><span data-stu-id="78de2-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="78de2-110">Expertul de instalare are nevoie de aceste informații pentru a configura corect agentul și a se asigura că poate comunica cu Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="78de2-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="78de2-111">[Împingeți date de diagnosticare în spațiul de lucru](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="78de2-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="78de2-112">Puteți să împingeți date de diagnosticare din entitatea găzduită WVD în Analiza jurnalelor pentru spațiul de lucru.</span><span class="sxs-lookup"><span data-stu-id="78de2-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="78de2-113">[Identificați și diagnosticați](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemele interne sau externe legate de WVD.</span><span class="sxs-lookup"><span data-stu-id="78de2-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="78de2-114">Pentru a afla mai multe despre configurarea instrumentului de diagnosticare a serviciului pentru WVD, consultați Utilizarea analizelor de jurnal pentru caracteristica de diagnosticare.</span><span class="sxs-lookup"><span data-stu-id="78de2-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>