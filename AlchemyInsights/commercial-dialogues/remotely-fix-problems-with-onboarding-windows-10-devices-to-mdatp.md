---
title: Remedierea de la distanță a problemelor cu dispozitivele Windows 10 la protecția avansată a amenințărilor la Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750040"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="78c11-102">Remedierea de la distanță a problemelor cu dispozitivele Windows 10 la protecția avansată a amenințărilor la Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="78c11-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="78c11-103">Dacă puteți accesa computerul la distanță, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="78c11-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="78c11-104">Descărcați instrumentul de diagnosticare [client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) .</span><span class="sxs-lookup"><span data-stu-id="78c11-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="78c11-105">Extrage și rulează MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="78c11-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="78c11-106">Găsiți Jurnalul de diagnosticare în folderul MDATPClientAnalyzerResult, care este același folder în care a fost descărcat instrumentul Analyzer.</span><span class="sxs-lookup"><span data-stu-id="78c11-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="78c11-107">Pentru a găsi probleme cu setările de conectivitate sau proxy de internet, examinați MDATPClientAnalyzer.txt fișierului jurnal.</span><span class="sxs-lookup"><span data-stu-id="78c11-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="78c11-108">Pentru a afla mai multe, consultați [probleme cu mașinile de la bord](https://go.microsoft.com/fwlink/?linkid=2143634).</span><span class="sxs-lookup"><span data-stu-id="78c11-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
