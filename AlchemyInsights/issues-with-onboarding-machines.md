---
title: Probleme cu înscrierea dispozitivelor la Microsoft Defender pentru Puncte Finale
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901579"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="14848-102">Probleme cu înscrierea dispozitivelor la Microsoft Defender pentru Puncte Finale</span><span class="sxs-lookup"><span data-stu-id="14848-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="14848-103">Este posibil să aveți probleme cu înscrierea dispozitivelor la serviciul MDE.</span><span class="sxs-lookup"><span data-stu-id="14848-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="14848-104">Dacă puteți accesa dispozitivul utilizatorului final, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="14848-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="14848-105">Descărcați cea mai recentă versiune preliminară a uneltei de diagnostic a [ Analizorului de Client MDE](https://aka.ms/betamdeanalyzer).</span><span class="sxs-lookup"><span data-stu-id="14848-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="14848-106">Faceți clic dreapta pe **MDEClientAnalyzer.cmd** și selectați "Rulare ca administrator".</span><span class="sxs-lookup"><span data-stu-id="14848-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="14848-107">Urmați instrucțiunile sugerate în **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="14848-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="14848-108">Pentru mai multe jurnale detaliate, revizuiți sub folderul creat, numit **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="14848-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="14848-109">Dacă sunt necesare instrucțiuni suplimentare, contactați [asistența Microsoft Defender pentru Punct Final](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) și furnizați fișierul MDEClientAnalyzerResult.zip care rezultă pentru analiză.</span><span class="sxs-lookup"><span data-stu-id="14848-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
