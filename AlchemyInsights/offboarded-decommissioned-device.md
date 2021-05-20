---
title: Probleme cu eliminarea unui dispozitiv eliminat din inventarul de dispozitive sau scos din depozit
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564606"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="2cf70-102">Probleme cu eliminarea unui dispozitiv eliminat din inventarul de dispozitive sau scos din depozit</span><span class="sxs-lookup"><span data-stu-id="2cf70-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="2cf70-103">Microsoft Defender pentru punctul final nu permite momentan eliminarea manuală a înregistrării dispozitivului pentru un dispozitiv înregistrat sau scos din inventarul de dispozitive.</span><span class="sxs-lookup"><span data-stu-id="2cf70-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="2cf70-104">Din motive de securitate, dispozitivul rămâne în portal ca înregistrare istorică timp de până la 180 de zile.</span><span class="sxs-lookup"><span data-stu-id="2cf70-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="2cf70-105">Cu toate acestea, datele dispozitivului sunt corectate conform perioadei de retenție configurate.</span><span class="sxs-lookup"><span data-stu-id="2cf70-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="2cf70-106">**Notă:** Un dispozitiv dezactivat sau scos din uz comută automat la **starea Inactiv** după șapte zile.</span><span class="sxs-lookup"><span data-stu-id="2cf70-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="2cf70-107">În plus, dispozitivele care nu sunt active în ultimele 30 de zile nu sunt factorate în datele care reflectă organizația dvs. Gestiunea amenințărilor și vulnerabilităților timpul de expunere sau Microsoft Secure Score pentru dispozitive.</span><span class="sxs-lookup"><span data-stu-id="2cf70-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="2cf70-108">Dacă tot nu doriți să vedeți anumite dispozitive în vizualizarea Inventar dispozitiv, încercați să plasați o etichetă de dispozitiv pentru a filtra dispozitivul scos din vedere din vizualizarea Inventar dispozitive.</span><span class="sxs-lookup"><span data-stu-id="2cf70-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="2cf70-109">Pentru mai multe informații, consultați:</span><span class="sxs-lookup"><span data-stu-id="2cf70-109">For more information, see:</span></span>

[<span data-ttu-id="2cf70-110">Offboard devices from the Microsoft Defender for Endpoint service</span><span class="sxs-lookup"><span data-stu-id="2cf70-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="2cf70-111">Score de expunere în Gestiunea amenințărilor și vulnerabilităților</span><span class="sxs-lookup"><span data-stu-id="2cf70-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="2cf70-112">Remedierea senzorilor nesă remediați în Microsoft Defender pentru punctul final</span><span class="sxs-lookup"><span data-stu-id="2cf70-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="2cf70-113">Cum să utilizați etichetarea eficient (Partea 1)</span><span class="sxs-lookup"><span data-stu-id="2cf70-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="2cf70-114">Cum să utilizați etichetarea eficient (Partea 2)</span><span class="sxs-lookup"><span data-stu-id="2cf70-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="2cf70-115">Cum să utilizați etichetarea eficient (Partea 3)</span><span class="sxs-lookup"><span data-stu-id="2cf70-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




