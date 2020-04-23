---
title: Remedierea erorii 0x8004de40 în OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716040"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="fa0ac-102">Remedierea erorii 0x8004de40 în OneDrive</span><span class="sxs-lookup"><span data-stu-id="fa0ac-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="fa0ac-103">Dacă primiți o eroare 0x8004de40 cu OneDrive:</span><span class="sxs-lookup"><span data-stu-id="fa0ac-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="fa0ac-104">Reporniți computerul afectat în timp ce conectat la domeniul Director Acitve.</span><span class="sxs-lookup"><span data-stu-id="fa0ac-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="fa0ac-105">Dacă o repornire nu remediază problema, unjoin și realăturați-vă dispozitivul de la Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fa0ac-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="fa0ac-106">**Notă:** Ar trebui să fie în rețeaua de corporate în timp ce efectuați acești pași.</span><span class="sxs-lookup"><span data-stu-id="fa0ac-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="fa0ac-107">Nu efectuați acești pași atunci când nu vă puteți conecta la infrastructura companiei (de exemplu, în timpul călătoriei).</span><span class="sxs-lookup"><span data-stu-id="fa0ac-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="fa0ac-108">Deschideți un prompt de comandă privilegiat.</span><span class="sxs-lookup"><span data-stu-id="fa0ac-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="fa0ac-109">Pentru a deschide un prompt de comandă privilegiat, faceți clic pe **Start**, faceți clic cu butonul din dreapta pe **Linie de comandă**, apoi faceți clic pe Executare ca **administrator**.</span><span class="sxs-lookup"><span data-stu-id="fa0ac-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="fa0ac-110">Tastați *dsregcmd /leave* și apăsați **Enter**.</span><span class="sxs-lookup"><span data-stu-id="fa0ac-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="fa0ac-111">Când terminați, tastați *dsregcmd /join* și apăsați **Enter**.</span><span class="sxs-lookup"><span data-stu-id="fa0ac-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="fa0ac-112">Când terminați, închideți promptul de comandă.</span><span class="sxs-lookup"><span data-stu-id="fa0ac-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="fa0ac-113">Reporniți computerul și conectați-vă la OneDrive.</span><span class="sxs-lookup"><span data-stu-id="fa0ac-113">Reboot the computer, and log into OneDrive.</span></span>