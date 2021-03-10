---
title: Offboard non-dispozitivele Windows de la Microsoft Defender-protecție avansată împotriva amenințărilor (ATP)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695157"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="b6e6e-102">Offboard non-dispozitivele Windows de la Microsoft Defender-protecție avansată împotriva amenințărilor (ATP)</span><span class="sxs-lookup"><span data-stu-id="b6e6e-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="b6e6e-103">Iată cum se procedează:</span><span class="sxs-lookup"><span data-stu-id="b6e6e-103">Here's how:</span></span>

1. <span data-ttu-id="b6e6e-104">Urmați documentația de la terți pentru deconectarea soluției de la terți de la Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="b6e6e-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="b6e6e-105">De la entitatea găzduită Azure Active Directory, eliminați permisiunile pentru soluția de la terți:</span><span class="sxs-lookup"><span data-stu-id="b6e6e-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="b6e6e-106">Conectați-vă la [portalul Azure](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="b6e6e-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="b6e6e-107">Selectare **totală servicii**  >  **Azure Active Directory**  >  **Enterprise Applications**.</span><span class="sxs-lookup"><span data-stu-id="b6e6e-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="b6e6e-108">Selectați aplicația pe care doriți să o offboard.</span><span class="sxs-lookup"><span data-stu-id="b6e6e-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="b6e6e-109">Selectați **Ștergere**.</span><span class="sxs-lookup"><span data-stu-id="b6e6e-109">Select **Delete**.</span></span>

<span data-ttu-id="b6e6e-110">Pentru a afla mai multe, consultați [offboard dispozitivelor non-Windows](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="b6e6e-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
