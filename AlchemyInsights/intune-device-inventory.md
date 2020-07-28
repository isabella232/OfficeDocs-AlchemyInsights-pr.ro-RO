---
title: Inventar dispozitiv Intune
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
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440474"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="a9188-102">Inventar dispozitiv Intune</span><span class="sxs-lookup"><span data-stu-id="a9188-102">Intune Device Inventory</span></span>

<span data-ttu-id="a9188-103">Lama Devices oferă administratorului o perspectivă asupra dispozitivelor aflate în administrare în Intune pe bază de dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="a9188-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="a9188-104">Informațiile afișate includ: Hardware, Aplicații descoperite, Starea de conformitate a dispozitivului și Starea configurației dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="a9188-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="a9188-105">Datele de inventar pentru hardware și aplicațiile descoperite sunt colectate pe un ciclu de șapte zile.</span><span class="sxs-lookup"><span data-stu-id="a9188-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="a9188-106">Aplicațiile și elementele specifice ale hardware-ului raportate diferă în funcție de sistemul de operare al dispozitivului și dacă dispozitivul este deținut personal sau de companie.</span><span class="sxs-lookup"><span data-stu-id="a9188-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="a9188-107">Pentru mai multe informații, consultați [Vedeți detaliile dispozitivului în Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="a9188-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="a9188-108">**ÎNTREBĂRI FRECVENTE**</span><span class="sxs-lookup"><span data-stu-id="a9188-108">**FAQ**</span></span>

<span data-ttu-id="a9188-109">Î: Nu primesc o listă completă de inventar a aplicațiilor prezente pe dispozitivele Windows încorporate intune.</span><span class="sxs-lookup"><span data-stu-id="a9188-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="a9188-110">de ce nu?</span><span class="sxs-lookup"><span data-stu-id="a9188-110">Why not?</span></span>

<span data-ttu-id="a9188-111">R: În acest moment, numai aplicațiile moderne sunt listate pentru PC-urile Windows 10 care sunt identificate ca dispozitive corporative.</span><span class="sxs-lookup"><span data-stu-id="a9188-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="a9188-112">Intune nu colectează informații despre aplicațiile Win32 instalate pe aceste dispozitive.</span><span class="sxs-lookup"><span data-stu-id="a9188-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="a9188-113">Î: De ce numerele de telefon nu sunt colectate de pe toate dispozitivele?</span><span class="sxs-lookup"><span data-stu-id="a9188-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="a9188-114">R: Telefoanele clasificate ca dispozitive corporative în Intune nu sunt identificate cu numărul lor de telefon complet atunci când, de exemplu, executați un raport de inventar al dispozitivului mobil.</span><span class="sxs-lookup"><span data-stu-id="a9188-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="a9188-115">Numerele de telefon ale dispozitivului Bring-you-own sunt întotdeauna parțial mascate cu asteriscuri (\*\*\*\*) și afișează doar ultimele patru cifre.</span><span class="sxs-lookup"><span data-stu-id="a9188-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>