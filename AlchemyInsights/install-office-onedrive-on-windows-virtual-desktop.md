---
title: Instalarea Office și OneDrive pe Desktop virtual Windows
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
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595842"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="c6052-102">Instalarea Office și OneDrive pe Desktop virtual Windows</span><span class="sxs-lookup"><span data-stu-id="c6052-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="c6052-103">[Pregătirea și particularizarea unei imagini VHD coordonatoare.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)</span><span class="sxs-lookup"><span data-stu-id="c6052-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="c6052-104">Creați o mașină virtuală (VM) dacă nu a fost creată deja.</span><span class="sxs-lookup"><span data-stu-id="c6052-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="c6052-105">[Instalați Office în modul de activare a computerului partajat.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)</span><span class="sxs-lookup"><span data-stu-id="c6052-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="c6052-106">Activarea computerului partajat permite mai multor utilizatori să acceseze Office.</span><span class="sxs-lookup"><span data-stu-id="c6052-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="c6052-107">[Instalați OneDrive în modul per computer](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span><span class="sxs-lookup"><span data-stu-id="c6052-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="c6052-108">În mod normal, OneDrive este instalat per utilizator, dar aici ar trebui să fie instalat pe computer.</span><span class="sxs-lookup"><span data-stu-id="c6052-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>