---
title: Fix 0x8004de40 eroare în OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052049"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="ef59e-102">Fix 0x8004de40 eroare în OneDrive</span><span class="sxs-lookup"><span data-stu-id="ef59e-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="ef59e-103">Dacă primiți o eroare 0x8004de40 cu OneDrive:</span><span class="sxs-lookup"><span data-stu-id="ef59e-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="ef59e-104">Reporniți computerul afectat în timp ce sunteți conectat la domeniul Acitve Directory.</span><span class="sxs-lookup"><span data-stu-id="ef59e-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="ef59e-105">Dacă o repornire nu remediază problema, părăsiţi și realăturați-vă dispozitivul de la Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ef59e-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="ef59e-106">**Notă**: ar trebui să fiți în rețeaua corporativă în timp ce efectuați acești pași.</span><span class="sxs-lookup"><span data-stu-id="ef59e-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="ef59e-107">Nu efectuați acești pași atunci când nu sunteți în măsură să vă conectați la infrastructura corporativă (de exemplu, în timp ce călătoriți).</span><span class="sxs-lookup"><span data-stu-id="ef59e-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="ef59e-108">Deschideți un prompt de comandă privilegiat.</span><span class="sxs-lookup"><span data-stu-id="ef59e-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="ef59e-109">Pentru a deschide un prompt de comandă privilegiat, faceți clic pe **Start**, faceți clic dreapta pe **Command Prompt**, apoi faceți clic pe **Executare ca administrator**.</span><span class="sxs-lookup"><span data-stu-id="ef59e-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="ef59e-110">Tip *dsregcmd/plecare* și pres **Enter**.</span><span class="sxs-lookup"><span data-stu-id="ef59e-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="ef59e-111">Când complet, tastați *dsregcmd/Join* și apăsați **Enter**.</span><span class="sxs-lookup"><span data-stu-id="ef59e-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="ef59e-112">Când terminați, închideți promptul de comandă.</span><span class="sxs-lookup"><span data-stu-id="ef59e-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="ef59e-113">Reporniți computerul și conectați-vă la OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ef59e-113">Reboot the computer, and log into OneDrive.</span></span>