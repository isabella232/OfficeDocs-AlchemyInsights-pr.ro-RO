---
title: Întreruperea actualizărilor programate
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555516"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="8505f-102">Întreruperea actualizărilor programate</span><span class="sxs-lookup"><span data-stu-id="8505f-102">Pausing scheduled updates</span></span>

<span data-ttu-id="8505f-103">Când se emite o comandă de pauză, dispozitivele nu procesează comanda până la următoarea check-in în Intune.</span><span class="sxs-lookup"><span data-stu-id="8505f-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="8505f-104">Din acest motiv, este posibil ca dispozitivele să aibă:</span><span class="sxs-lookup"><span data-stu-id="8505f-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="8505f-105">S-au instalat actualizările programate înainte de check-in.</span><span class="sxs-lookup"><span data-stu-id="8505f-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="8505f-106">A fost oprit când ați emis comanda pauză.</span><span class="sxs-lookup"><span data-stu-id="8505f-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="8505f-107">În acest caz, când dispozitivele au fost pornite, este posibil să fi descărcat și instalat actualizările programate înainte de check-in.</span><span class="sxs-lookup"><span data-stu-id="8505f-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>