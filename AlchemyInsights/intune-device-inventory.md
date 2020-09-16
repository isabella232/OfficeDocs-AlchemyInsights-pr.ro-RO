---
title: Inventarul dispozitivelor Intune
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
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667890"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="fb957-102">Inventarul dispozitivelor Intune</span><span class="sxs-lookup"><span data-stu-id="fb957-102">Intune Device Inventory</span></span>

<span data-ttu-id="fb957-103">Lama Devices oferă administratorului informații despre dispozitivele de sub gestionare în Intune pe bază de dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="fb957-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="fb957-104">Informațiile afișate includ: hardware, aplicații descoperite, starea conformității dispozitivelor și starea configurației dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="fb957-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="fb957-105">Datele de inventar pentru componente hardware și aplicații descoperite sunt colectate pe un ciclu de șapte zile.</span><span class="sxs-lookup"><span data-stu-id="fb957-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="fb957-106">Aplicațiile și elementele specifice ale componentelor hardware raportate diferă în funcție de sistemul de operare al dispozitivului și dacă dispozitivul este deținut personal sau corporativ.</span><span class="sxs-lookup"><span data-stu-id="fb957-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="fb957-107">Pentru mai multe informații, consultați [Vedeți detaliile dispozitivului în Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="fb957-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="fb957-108">**ÎNTREBĂRI FRECVENTE**</span><span class="sxs-lookup"><span data-stu-id="fb957-108">**FAQ**</span></span>

<span data-ttu-id="fb957-109">Î: nu primesc o listă completă de inventar a aplicațiilor prezente pe dispozitivele Windows Intune-inrolat.</span><span class="sxs-lookup"><span data-stu-id="fb957-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="fb957-110">de ce nu?</span><span class="sxs-lookup"><span data-stu-id="fb957-110">Why not?</span></span>

<span data-ttu-id="fb957-111">A: în acest moment, doar aplicațiile moderne sunt listate pentru PC-urile Windows 10 care sunt identificate ca dispozitive corporative.</span><span class="sxs-lookup"><span data-stu-id="fb957-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="fb957-112">Intune nu colectează informații despre aplicațiile Win32 instalate pe aceste dispozitive.</span><span class="sxs-lookup"><span data-stu-id="fb957-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="fb957-113">Î: de ce nu sunt colectate numerele de telefon de pe toate dispozitivele?</span><span class="sxs-lookup"><span data-stu-id="fb957-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="fb957-114">A: telefoanele clasificate ca dispozitive corporative în Intune nu sunt identificate cu numărul de telefon complet atunci când, de exemplu, rulează un raport de inventar al dispozitivelor mobile.</span><span class="sxs-lookup"><span data-stu-id="fb957-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="fb957-115">Numerele de telefon bring-you-own-dispozitiv sunt întotdeauna parțial mascate cu asteriscuri (\* \* \* \*) și afișează doar ultimele patru cifre.</span><span class="sxs-lookup"><span data-stu-id="fb957-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>