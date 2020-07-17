---
title: Probleme cu mașinile de îmbarcare
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141658"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="1a50f-102">Probleme cu mașinile de îmbarcare</span><span class="sxs-lookup"><span data-stu-id="1a50f-102">Issues with onboarding machines</span></span>

<span data-ttu-id="1a50f-103">Este posibil să aveți probleme cu mașinile de îmbarcare pentru serviciul MDATP.</span><span class="sxs-lookup"><span data-stu-id="1a50f-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="1a50f-104">Dacă puteți accesa computerul utilizatorului final, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="1a50f-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="1a50f-105">Descărcați instrumentul de diagnosticare [Client Connectivity Analyzer.](https://aka.ms/mdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="1a50f-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="1a50f-106">Extrageți și executați MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="1a50f-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="1a50f-107">Găsiți jurnalul de diagnosticare în folderul numit MDATPClientAnalyzerResult, același folder în care este descărcat instrumentul Analyzer.</span><span class="sxs-lookup"><span data-stu-id="1a50f-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="1a50f-108">Examinați fișierul jurnal, MDATPClientAnalyzer.txt, pentru a găsi probleme de conectivitate sau setări proxy internet.</span><span class="sxs-lookup"><span data-stu-id="1a50f-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>