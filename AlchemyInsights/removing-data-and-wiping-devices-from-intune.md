---
title: Eliminarea datelor și ștergerea dispozitivelor din Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440469"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="df17d-102">Eliminarea datelor și ștergerea dispozitivelor din Intune</span><span class="sxs-lookup"><span data-stu-id="df17d-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="df17d-103">Acțiunile de la distanță Pentru retragerea dispozitivului și ștergerea dispozitivului pot fi utilizate pentru a elimina datele companiei gestionate de Intune sau pentru a efectua o resetare din fabrică și pentru a readuce dispozitivul la setările sale implicite.</span><span class="sxs-lookup"><span data-stu-id="df17d-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="df17d-104">Conectați-vă la Microsoft 365 **Devices**Device Management și accesați  >  **Devices All Devices**.</span><span class="sxs-lookup"><span data-stu-id="df17d-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="df17d-105">Selectați dispozitivul pe care doriți să-l ștergeți.</span><span class="sxs-lookup"><span data-stu-id="df17d-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="df17d-106">Selectați tipul de ștergere la distanță pe care doriți să îl faceți.</span><span class="sxs-lookup"><span data-stu-id="df17d-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="df17d-107">Retragere șterge numai informațiile organizaționale, în timp ce șervețelele complete restabilesc dispozitivul la setările sale din fabrică.</span><span class="sxs-lookup"><span data-stu-id="df17d-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="df17d-108">Selectați **Da** pentru confirmare.</span><span class="sxs-lookup"><span data-stu-id="df17d-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="df17d-109">Până la terminarea ștergerii, starea acțiunii Dispozitiv se afișează ca Retragere în așteptare.</span><span class="sxs-lookup"><span data-stu-id="df17d-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="df17d-110">După terminarea acțiunii, nu veți mai vedea dispozitivul mobil în lista de dispozitive gestionate.</span><span class="sxs-lookup"><span data-stu-id="df17d-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="df17d-111">**Notă** Datele companiei nu pot fi eliminate de pe dispozitivele ASOCIATE în Azure AD.</span><span class="sxs-lookup"><span data-stu-id="df17d-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="df17d-112">Pentru detalii complete despre efectul acțiunilor Retragere și ștergere, inclusiv ce este reținut și ce este șters, consultați [Eliminarea dispozitivelor utilizând ștergerea, retragerea sau anularea manuală a dispozitivului](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="df17d-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="df17d-113">Pentru a șterge toate datele de pe un dispozitiv macOS, consultați [Ștergerea tuturor datelor de pe un dispozitiv macOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="df17d-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>