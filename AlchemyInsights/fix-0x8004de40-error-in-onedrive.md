---
title: Remedierea erorii 0x8004de40 în OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745142"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="5fab0-102">Remedierea erorii 0x8004de40 în OneDrive</span><span class="sxs-lookup"><span data-stu-id="5fab0-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="5fab0-103">Dacă primiți o eroare 0x8004de40 cu OneDrive:</span><span class="sxs-lookup"><span data-stu-id="5fab0-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="5fab0-104">Reporniți computerul afectat în timp ce sunteți conectat la domeniul directorului Acitve.</span><span class="sxs-lookup"><span data-stu-id="5fab0-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="5fab0-105">Dacă repornirea nu rezolvă problema, anulați asocierea și reasocierea dispozitivului din Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5fab0-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="5fab0-106">**Notă**: trebuie să fiți în rețeaua corporativă în timp ce efectuați acești pași.</span><span class="sxs-lookup"><span data-stu-id="5fab0-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="5fab0-107">Nu efectuați acești pași atunci când nu vă puteți conecta la infrastructura firmei (de exemplu, în timpul călătoriei).</span><span class="sxs-lookup"><span data-stu-id="5fab0-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="5fab0-108">Deschideți un prompt de comandă privilegiat.</span><span class="sxs-lookup"><span data-stu-id="5fab0-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="5fab0-109">Pentru a deschide o linie de comandă privilegiat, faceți clic pe- **Start**, faceți clic dreapta pe **linie de comandă**, apoi faceți clic pe **rulare ca administrator**.</span><span class="sxs-lookup"><span data-stu-id="5fab0-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="5fab0-110">Tastați *dsregcmd/Leave* și apăsați pe **Enter**.</span><span class="sxs-lookup"><span data-stu-id="5fab0-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="5fab0-111">Când terminați, tastați *dsregcmd/Join* și apăsați pe **Enter**.</span><span class="sxs-lookup"><span data-stu-id="5fab0-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="5fab0-112">Când terminați, închideți linia de comandă.</span><span class="sxs-lookup"><span data-stu-id="5fab0-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="5fab0-113">Reporniți computerul și conectați-vă la OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5fab0-113">Reboot the computer, and log into OneDrive.</span></span>