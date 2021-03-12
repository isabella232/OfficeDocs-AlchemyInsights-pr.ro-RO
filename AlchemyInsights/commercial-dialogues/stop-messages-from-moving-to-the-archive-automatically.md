---
title: Oprirea automată a mesajelor în arhivă
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
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749823"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="1ab13-102">Oprirea automată a mesajelor în arhivă</span><span class="sxs-lookup"><span data-stu-id="1ab13-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="1ab13-103">Dacă utilizați o politică de retenție, puteți modifica vârsta de retenție din acea politică pentru a opri automat mesajele să se arhiveze.</span><span class="sxs-lookup"><span data-stu-id="1ab13-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="1ab13-104">Iată cum se procedează:</span><span class="sxs-lookup"><span data-stu-id="1ab13-104">Here's how:</span></span>

1. <span data-ttu-id="1ab13-105">În [Centrul de administrare Exchange](https://go.microsoft.com/fwlink/?linkid=2059104), alegeți etichete de retenție pentru **gestionarea conformității**  >  .</span><span class="sxs-lookup"><span data-stu-id="1ab13-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="1ab13-106">Găsiți mutarea pentru a arhiva eticheta de retenție.</span><span class="sxs-lookup"><span data-stu-id="1ab13-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="1ab13-107">În eticheta retenție, modificați perioada de retenție (perioada de arhivare) pentru a **nu opri niciodată** elementele să fie arhivate automat de o politică de retenție.</span><span class="sxs-lookup"><span data-stu-id="1ab13-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="1ab13-108">Astfel, se va modifica setarea arhivă pentru toate cutiile poștale cu această etichetă de retenție aplicată.</span><span class="sxs-lookup"><span data-stu-id="1ab13-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
