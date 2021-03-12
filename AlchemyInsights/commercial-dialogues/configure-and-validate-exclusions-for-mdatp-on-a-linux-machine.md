---
title: Configurarea și validarea excluderilor pentru MDATP pe o mașină Linux
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749251"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="0fc9a-102">Configurarea și validarea excluderilor pentru MDATP pe o mașină Linux</span><span class="sxs-lookup"><span data-stu-id="0fc9a-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="0fc9a-103">Puteți să excludeți anumite fișiere, foldere, procese și fișiere deschise proceselor din scanări MDATP.</span><span class="sxs-lookup"><span data-stu-id="0fc9a-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="0fc9a-104">Excluderi ajuta la prevenirea detectării incorecte a software-ului și a fișierelor unice sau particularizate pentru organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="0fc9a-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="0fc9a-105">Excluderi ajută, de asemenea, la atenuarea problemelor de performanță cauzate de MDATP.</span><span class="sxs-lookup"><span data-stu-id="0fc9a-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="0fc9a-106">Pentru a afla mai multe, consultați [Configurarea și validarea excluderilor pentru MDATP pentru Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="0fc9a-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0fc9a-107">Excluderile descrise în acest articol nu se aplică altor capacități de MDATP pentru Linux, inclusiv detectarea punctului final și răspunsul (EDR).</span><span class="sxs-lookup"><span data-stu-id="0fc9a-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="0fc9a-108">Fișierele pe care le excludeți prin utilizarea metodelor descrise în acest articol pot totuși să declanșeze avertizări EDR și alte capacități de detectare.</span><span class="sxs-lookup"><span data-stu-id="0fc9a-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
