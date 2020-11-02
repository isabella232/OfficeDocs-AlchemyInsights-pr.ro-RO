---
title: eroare 0x8004de40 atunci când lansați OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823115"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="de7cd-102">eroare 0x8004de40 atunci când lansați OneDrive</span><span class="sxs-lookup"><span data-stu-id="de7cd-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="de7cd-103">Dacă primiți o eroare **0x8004de40** atunci când vă conectați la OneDrive, reporniți computerul în timp ce sunteți conectat la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="de7cd-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="de7cd-104">Dacă primiți această eroare după repornirea acestuia, încercați acest lucru în timp ce sunteți conectat la domeniul de la locul de muncă sau de la școală:</span><span class="sxs-lookup"><span data-stu-id="de7cd-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="de7cd-105">Faceți clic pe Start și tastați **cmd** sau **promptul de comandă**  în caseta de căutare, faceți clic cu butonul din dreapta pe aplicația linie de comandă și selectați  **rulare ca administrator** .</span><span class="sxs-lookup"><span data-stu-id="de7cd-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="de7cd-106">Dacă vi se solicită o parolă de administrator sau o confirmare, tastați parola sau faceți clic pe se **permite** .</span><span class="sxs-lookup"><span data-stu-id="de7cd-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="de7cd-107">În fereastra linie de comandă, tastați **dsregcmd/Leave**  și așteptați ca comanda să se termine.</span><span class="sxs-lookup"><span data-stu-id="de7cd-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="de7cd-108">Apoi tastați **dsregcmd/Join** și așteptați ca comanda să se termine.</span><span class="sxs-lookup"><span data-stu-id="de7cd-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="de7cd-109">Reporniți computerul.</span><span class="sxs-lookup"><span data-stu-id="de7cd-109">Reboot your computer.</span></span>
