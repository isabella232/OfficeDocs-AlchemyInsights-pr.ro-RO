---
title: Starea senzorului pentru punctul final Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676339"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="eba36-102">Starea senzorului pentru punctul final Defender</span><span class="sxs-lookup"><span data-stu-id="eba36-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="eba36-103">Dala **Dispozitive cu probleme de** senzor se află pe tabloul de bord Operațiuni de securitate.</span><span class="sxs-lookup"><span data-stu-id="eba36-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="eba36-104">Această dală furnizează informații despre capacitatea dispozitivului individual de a furniza date despre senzor și de a comunica cu serviciul Defender pentru puncte finale.</span><span class="sxs-lookup"><span data-stu-id="eba36-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="eba36-105">Acesta raportează câte dispozitive necesită atenție și vă ajută să identificați dispozitivele problematice și să luați măsuri pentru a corecta problemele cunoscute.</span><span class="sxs-lookup"><span data-stu-id="eba36-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="eba36-106">Doi indicatori de stare ai dalei furnizează informații despre numărul de dispozitive care nu raportează corect serviciul:</span><span class="sxs-lookup"><span data-stu-id="eba36-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="eba36-107">**Configurați greșit** Dispozitivele care pot fi parțial de raportare a datelor despre senzor la serviciul Defender pentru punctul final și care pot avea erori de configurare care trebuie corectate.</span><span class="sxs-lookup"><span data-stu-id="eba36-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="eba36-108">**Inactiv** Dispozitivele care au oprit raportarea la serviciul Defender pentru puncte finale mai mult de șapte zile în ultima lună.</span><span class="sxs-lookup"><span data-stu-id="eba36-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="eba36-109">Un clic pe oricare dintre grupuri vă direcționează către lista Dispozitive, filtrată după opțiunile dvs.</span><span class="sxs-lookup"><span data-stu-id="eba36-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="eba36-110">În lista Dispozitive, puteți filtra lista cu starea de bună stare după următoarea stare:</span><span class="sxs-lookup"><span data-stu-id="eba36-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="eba36-111">**Activ** Dispozitive care raportează în mod activ la serviciul Defender pentru puncte finale.</span><span class="sxs-lookup"><span data-stu-id="eba36-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="eba36-112">**Configurați greșit** Dispozitivele care pot fi parțial de raportare a datelor despre senzor la serviciul Defender pentru punctul final, dar au erori de configurare care trebuie corectate.</span><span class="sxs-lookup"><span data-stu-id="eba36-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="eba36-113">Dispozitivele configurate greșit pot avea una sau o combinație a următoarelor probleme:</span><span class="sxs-lookup"><span data-stu-id="eba36-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="eba36-114">Fără date despre senzor - Dispozitivele nu mai trimit date despre senzor.</span><span class="sxs-lookup"><span data-stu-id="eba36-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="eba36-115">Avertizările limitate se pot declanșa de pe dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="eba36-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="eba36-116">Comunicații cu deficiențe - Capacitatea de a comunica cu dispozitivul este afectată.</span><span class="sxs-lookup"><span data-stu-id="eba36-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="eba36-117">Trimiterea de fișiere pentru analiză aprofundată, blocarea fișierelor, blocarea dispozitivului din rețea și alte acțiuni care necesită comunicarea cu dispozitivul pot să nu funcționează.</span><span class="sxs-lookup"><span data-stu-id="eba36-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="eba36-118">**Inactiv** Dispozitivele care au oprit raportarea la serviciul Defender pentru punct final.</span><span class="sxs-lookup"><span data-stu-id="eba36-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="eba36-119">Puteți descărca întreaga listă în format CSV utilizând caracteristica Export.</span><span class="sxs-lookup"><span data-stu-id="eba36-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="eba36-120">Pentru mai multe informații, consultați [Verificarea stării stării senzorului în Microsoft Defender pentru punctul final.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="eba36-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="eba36-121">Pentru mai multe informații despre cauza inactivă sau configurarea greșită a unui dispozitiv, consultați Remedierea senzorilor ne sănătos în [Microsoft Defender pentru punctul final.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)</span><span class="sxs-lookup"><span data-stu-id="eba36-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
