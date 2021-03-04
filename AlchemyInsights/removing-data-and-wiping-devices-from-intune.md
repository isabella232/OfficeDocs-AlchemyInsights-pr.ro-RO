---
title: Eliminarea datelor și ștergerea dispozitivelor din Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416325"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="3c2e7-102">Eliminarea datelor și ștergerea dispozitivelor din Intune</span><span class="sxs-lookup"><span data-stu-id="3c2e7-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="3c2e7-103">Acțiunile la distanță de retragere și ștergere a dispozitivului pot fi utilizate pentru a elimina datele firmei gestionate de Intune sau pentru a efectua o reinițializare la setările din fabrică și a restabili setările implicite pe dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="3c2e7-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="3c2e7-104">Conectați-vă la Microsoft 365 Management și accesați **Dispozitive** > **Toate dispozitivele**.</span><span class="sxs-lookup"><span data-stu-id="3c2e7-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="3c2e7-105">Selectați dispozitivul pe care doriți să îl ștergeți.</span><span class="sxs-lookup"><span data-stu-id="3c2e7-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="3c2e7-106">Selectați tipul de ștergere de la distanță pe care doriți să o efectuați.</span><span class="sxs-lookup"><span data-stu-id="3c2e7-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="3c2e7-107">Retragerea șterge numai informațiile organizației, în timp ce ștergerile complete restaurează dispozitivul la setările din fabrică.</span><span class="sxs-lookup"><span data-stu-id="3c2e7-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="3c2e7-108">Selectați **Da** pentru a confirma.</span><span class="sxs-lookup"><span data-stu-id="3c2e7-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="3c2e7-109">Până când se termină ștergerea, starea acțiunii pentru dispozitiv se afișează ca *În aşteptarea retragerii*.</span><span class="sxs-lookup"><span data-stu-id="3c2e7-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="3c2e7-110">După ce se încheie acțiunea, nu veți mai vedea dispozitivul mobil în lista de dispozitive gestionate.</span><span class="sxs-lookup"><span data-stu-id="3c2e7-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="3c2e7-111">Datele firmei nu pot fi eliminate de pe dispozitivele ASOCIATE la Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3c2e7-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="3c2e7-112">Pentru detalii complete cu privire la efectul acțiunilor de retragere și ștergere, inclusiv elementele păstrate și cele șterse, consultați documentația următoare:</span><span class="sxs-lookup"><span data-stu-id="3c2e7-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="3c2e7-113">[Eliminarea dispozitivelor utilizând ștergerea, retragerea sau anularea manuală a înscrierii dispozitivului](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="3c2e7-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="3c2e7-114">Cum să ștergeți doar datele corporației din aplicațiile gestionate de Intune</span><span class="sxs-lookup"><span data-stu-id="3c2e7-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="3c2e7-115">[Ștergeți toate datele de pe un dispozitiv macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="3c2e7-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>