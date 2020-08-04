---
title: Curățarea automată a dispozitivelor învechite în Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555228"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="b1469-102">Curățarea automată a dispozitivelor învechite în Intune</span><span class="sxs-lookup"><span data-stu-id="b1469-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="b1469-103">Intune permite administratorului să configureze un interval de timp între 90 și 270 de zile, după care dispozitivele învechite sunt eliminate din serviciu.</span><span class="sxs-lookup"><span data-stu-id="b1469-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="b1469-104">Această setare este la nivel de organizare și o dată activat intră în vigoare imediat.</span><span class="sxs-lookup"><span data-stu-id="b1469-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="b1469-105">Toate dispozitivele care nu au fost verificate în serverul Intune pentru o perioadă care depășește setarea sunt șterse definitiv.</span><span class="sxs-lookup"><span data-stu-id="b1469-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="b1469-106">**Notă** Numai obiectele de dispozitiv MDM sunt eligibile pentru această acțiune de curățare.</span><span class="sxs-lookup"><span data-stu-id="b1469-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="b1469-107">Sunt excluse numai obiectele dispozitivului EAS.</span><span class="sxs-lookup"><span data-stu-id="b1469-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="b1469-108">Pentru informații suplimentare despre momentul în care un dispozitiv devine eligibil pentru ștergere pe baza setării de curățare a dispozitivului și a "stării" acestuia:</span><span class="sxs-lookup"><span data-stu-id="b1469-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="b1469-109">Setare: **Ștergerea dispozitivelor după ultima dată de check-in: Da (o anumită valoare (N) în zilele specificate)**</span><span class="sxs-lookup"><span data-stu-id="b1469-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="b1469-110">Pe baza valorii (N) configurate în setare, serviciul Intune șterge dispozitivul în zilele specificate după ultima verificare reușită.</span><span class="sxs-lookup"><span data-stu-id="b1469-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="b1469-111">Setare: **Ștergerea dispozitivelor după ultima dată de check-in: Nu**</span><span class="sxs-lookup"><span data-stu-id="b1469-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="b1469-112">La 180 de zile de la expirarea certificatului dispozitivului și nu este reînnoit, dispozitivul este șters.</span><span class="sxs-lookup"><span data-stu-id="b1469-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="b1469-113">**Notă** În ambele cazuri, dispozitivul trebuie înregistrat cu succes în Intune.</span><span class="sxs-lookup"><span data-stu-id="b1469-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="b1469-114">Înregistrarea are loc în timpul primei verificări a dispozitivului cu serviciul Intune.</span><span class="sxs-lookup"><span data-stu-id="b1469-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="b1469-115">Dacă un dispozitiv se înscrie cu succes la Intune, dar nu devine înregistrat Intune, dispozitivul este șters la 270 de zile de la înscriere.</span><span class="sxs-lookup"><span data-stu-id="b1469-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="b1469-116">(90 de zile pentru a marca dispozitivul ca revocat, apoi alte 180 de zile pentru a șterge înregistrarea.)</span><span class="sxs-lookup"><span data-stu-id="b1469-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="b1469-117">Nu există niciun mecanism în prezent în consola Intune pentru a stabili data de expirare a certificării dispozitivului pentru un anumit dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="b1469-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>