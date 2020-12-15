---
title: Instrument de diagnosticare a serviciului pentru desktopul virtual Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680229"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="6f5ff-102">Instrument de diagnosticare a serviciului pentru desktopul virtual Windows</span><span class="sxs-lookup"><span data-stu-id="6f5ff-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="6f5ff-103">Desktopul virtual Windows (WVD) oferă un instrument de diagnosticare care permite administratorilor să identifice erorile printr-o singură interfață.</span><span class="sxs-lookup"><span data-stu-id="6f5ff-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="6f5ff-104">Acest instrument înregistrează informații legate de diagnosticare de fiecare dată când WVD este utilizat de o persoană atribuită un rol WVD.</span><span class="sxs-lookup"><span data-stu-id="6f5ff-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="6f5ff-105">Fiecare jurnal conține informații despre rolul WVD implicat în activitate, mesajele de eroare care apar în timpul sesiunii și informațiile despre entitatea găzduită și utilizator.</span><span class="sxs-lookup"><span data-stu-id="6f5ff-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="6f5ff-106">Analizele de jurnal Azure pot fi configurate pentru a captura Jurnalul de activități creat de instrumentul de diagnosticare.</span><span class="sxs-lookup"><span data-stu-id="6f5ff-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="6f5ff-107">Iată cum se procedează:</span><span class="sxs-lookup"><span data-stu-id="6f5ff-107">Here's how:</span></span>

1. <span data-ttu-id="6f5ff-108">Creați un spațiu de lucru de analiză jurnal cu [portalul Azure](https://go.microsoft.com/fwlink/?linkid=2129500) sau [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="6f5ff-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="6f5ff-109">[Conectați computerele Windows la Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="6f5ff-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="6f5ff-110">Obțineți ID-ul spațiului de lucru și cheia principală a spațiului de lucru.</span><span class="sxs-lookup"><span data-stu-id="6f5ff-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="6f5ff-111">Expertul de configurare are nevoie de aceste informații pentru a configura corect agentul și pentru a vă asigura că poate comunica cu Azure monitor.</span><span class="sxs-lookup"><span data-stu-id="6f5ff-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="6f5ff-112">[Împingeți datele de diagnosticare în spațiul de lucru](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="6f5ff-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="6f5ff-113">Puteți să deconectați datele de diagnosticare de la entitatea găzduită WVD la analizele jurnal pentru spațiul de lucru.</span><span class="sxs-lookup"><span data-stu-id="6f5ff-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="6f5ff-114">[Identificați și diagnosticați problemele](https://go.microsoft.com/fwlink/?linkid=2128338) care sunt interne sau externe în legătură cu WVD.</span><span class="sxs-lookup"><span data-stu-id="6f5ff-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="6f5ff-115">Pentru a afla mai multe despre configurarea instrumentului de diagnosticare a serviciului pentru WVD, consultați [utilizarea analizei jurnal pentru caracteristica de diagnosticare](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="6f5ff-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
