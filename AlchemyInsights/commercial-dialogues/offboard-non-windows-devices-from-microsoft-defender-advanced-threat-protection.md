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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748480"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="c24bb-102">Offboard non-dispozitivele Windows de la Microsoft Defender-protecție avansată împotriva amenințărilor (ATP)</span><span class="sxs-lookup"><span data-stu-id="c24bb-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="c24bb-103">Iată cum se procedează:</span><span class="sxs-lookup"><span data-stu-id="c24bb-103">Here's how:</span></span>

1. <span data-ttu-id="c24bb-104">Urmați documentația de la terți pentru deconectarea soluției de la terți de la Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="c24bb-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="c24bb-105">De la entitatea găzduită Azure Active Directory, eliminați permisiunile pentru soluția de la terți:</span><span class="sxs-lookup"><span data-stu-id="c24bb-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="c24bb-106">Conectați-vă la [portalul Azure](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="c24bb-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="c24bb-107">Selectare **totală servicii**  >  **Azure Active Directory**  >  **Enterprise Applications**.</span><span class="sxs-lookup"><span data-stu-id="c24bb-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="c24bb-108">Selectați aplicația pe care doriți să o offboard.</span><span class="sxs-lookup"><span data-stu-id="c24bb-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="c24bb-109">Selectați **Ștergere**.</span><span class="sxs-lookup"><span data-stu-id="c24bb-109">Select **Delete**.</span></span>

<span data-ttu-id="c24bb-110">Pentru a afla mai multe, consultați [offboard dispozitivelor non-Windows](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="c24bb-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
