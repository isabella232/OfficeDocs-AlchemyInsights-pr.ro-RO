---
title: Fix 0x8004de40 eroare în OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133988"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="1ee98-102">Fix 0x8004de40 eroare în OneDrive</span><span class="sxs-lookup"><span data-stu-id="1ee98-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="1ee98-103">Dacă primiţi o eroare de 0x8004de40 cu OneDrive:</span><span class="sxs-lookup"><span data-stu-id="1ee98-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="1ee98-104">Reporniţi computerul afectat în timp ce conectat la domeniu Acitve Director.</span><span class="sxs-lookup"><span data-stu-id="1ee98-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="1ee98-105">În cazul în care o repornire nu se rezolvă problema, părăsiţi şi va reintra în aparatul de Azur AD.</span><span class="sxs-lookup"><span data-stu-id="1ee98-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="1ee98-106">**Notă**: ar trebui să fie pe reţeaua corporativă în timp ce efectuaţi aceşti paşi.</span><span class="sxs-lookup"><span data-stu-id="1ee98-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="1ee98-107">Nu efectuaţi aceşti paşi, atunci când nu sunteţi capabil să se conecteze la infrastructurii corporative (de exemplu, în timp ce călătoresc).</span><span class="sxs-lookup"><span data-stu-id="1ee98-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="1ee98-108">Deschidere un ascensor virgulă prompt.</span><span class="sxs-lookup"><span data-stu-id="1ee98-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="1ee98-109">Pentru a deschide un prompt de comandă, faceţi clic pe - **Start**, faceţi clic dreapta pe **Prompt comandă**şi apoi faceţi clic pe **Executare ca administrator**.</span><span class="sxs-lookup"><span data-stu-id="1ee98-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="1ee98-110">*Dsregcmd /leave* de tip şi apăsaţi **Enter**.</span><span class="sxs-lookup"><span data-stu-id="1ee98-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="1ee98-111">Atunci când completă, tastaţi *dsregcmd/Join* şi apăsaţi **Enter**.</span><span class="sxs-lookup"><span data-stu-id="1ee98-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="1ee98-112">Când complet, închide promptul de comandă.</span><span class="sxs-lookup"><span data-stu-id="1ee98-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="1ee98-113">Reporniţi computerul, şi intraţi în OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1ee98-113">Reboot the computer, and log into OneDrive.</span></span>