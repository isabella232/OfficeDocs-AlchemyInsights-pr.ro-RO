---
title: 0x8004de40 la lansarea OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813664"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="5716b-102">0x8004de40 la lansarea OneDrive</span><span class="sxs-lookup"><span data-stu-id="5716b-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="5716b-103">Dacă primiți un mesaj de eroare **0x8004de40** atunci când vă conectați la OneDrive, reporniți computerul în timp ce sunteți conectat la domeniul de la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="5716b-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="5716b-104">Dacă primiți această eroare după repornire, încercați aceasta în timp ce sunteți conectat la domeniul de la locul de muncă sau de la școală:</span><span class="sxs-lookup"><span data-stu-id="5716b-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="5716b-105">Faceți clic pe Start și **tastați cmd** sau **linie** de comandă în caseta de căutare, faceți clic dreapta pe aplicația linie de comandă și **selectați Rulare ca administrator.**</span><span class="sxs-lookup"><span data-stu-id="5716b-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="5716b-106">Dacă vi se solicită o parolă de administrator sau o confirmare, tastați parola sau faceți clic pe **Se permite**.</span><span class="sxs-lookup"><span data-stu-id="5716b-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="5716b-107">În fereastra Linie de comandă, tastați **dsregcmd /leave și**  așteptați să se termine comanda.</span><span class="sxs-lookup"><span data-stu-id="5716b-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="5716b-108">Apoi tastați **dsregcmd /join** și așteptați comanda să se termine.</span><span class="sxs-lookup"><span data-stu-id="5716b-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="5716b-109">Reporniți computerul.</span><span class="sxs-lookup"><span data-stu-id="5716b-109">Reboot your computer.</span></span>
