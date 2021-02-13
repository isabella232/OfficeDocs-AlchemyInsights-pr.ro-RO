---
title: Adăugarea Microsoft Edge la Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194573"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="153da-102">Adăugarea Microsoft Edge la Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="153da-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="153da-103">Pentru a putea implementa, configura, monitoriza și proteja Microsoft Edge pentru Windows 10, trebuie mai întâi să îl adăugați la Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="153da-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="153da-104">Intune acceptă Microsoft Edge 77 și versiuni mai recente.</span><span class="sxs-lookup"><span data-stu-id="153da-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="153da-105">Intune va detecta toate instalările pre-existente din Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="153da-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="153da-106">Dacă Microsoft Edge este instalat în contextul utilizatorului, o instalare de sistem va suprascrie instalarea în contextul utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="153da-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="153da-107">Dacă Microsoft Edge este instalat în contextul sistemului, se va raporta succesul instalării.</span><span class="sxs-lookup"><span data-stu-id="153da-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="153da-108">Pre-instalat Microsoft Edge 77 și versiunile mai recente, pentru toate canalele din contextul utilizatorului, vor fi suprascrise cu Microsoft Edge instalat în contextul sistemului.</span><span class="sxs-lookup"><span data-stu-id="153da-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="153da-109">**Condiție**</span><span class="sxs-lookup"><span data-stu-id="153da-109">**Prerequisite**</span></span>

<span data-ttu-id="153da-110">Windows 10 versiunea 1709 sau versiuni mai recente</span><span class="sxs-lookup"><span data-stu-id="153da-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="153da-111">**Pașii pentru a adăuga Edge la Intune**</span><span class="sxs-lookup"><span data-stu-id="153da-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="153da-112">[Configurați aplicația în Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="153da-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="153da-113">[Configurați informațiile despre aplicație](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="153da-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="153da-114">[Configurați setările aplicației](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="153da-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="153da-115">[Selectați etichetele de domeniu (opțional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="153da-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="153da-116">[Adăugați aplicația](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="153da-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="153da-117">Pentru mai mult ajutor, consultați [Depanarea](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="153da-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




