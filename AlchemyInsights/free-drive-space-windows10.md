---
title: Eliberați spațiu pe disc în Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505368"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="c87c8-102">Eliberați spațiu pe disc în Windows 10</span><span class="sxs-lookup"><span data-stu-id="c87c8-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="c87c8-103">Iată două opțiuni pentru a elibera spațiu pe disc în Windows:</span><span class="sxs-lookup"><span data-stu-id="c87c8-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="c87c8-104">Eliberați spațiu pe disc în Windows 10.</span><span class="sxs-lookup"><span data-stu-id="c87c8-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="c87c8-105">Eliberați spațiu pentru actualizările Windows 10 cu dispozitivul de stocare extern.</span><span class="sxs-lookup"><span data-stu-id="c87c8-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="c87c8-106">Dacă aveți în continuare spațiu pe disc redus după ce utilizați Curățare disc, este posibil ca folderul Temp să se umple rapid cu fișiere de aplicație (.appx) utilizate de Magazinul Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c87c8-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="c87c8-107">Pentru a remedia această problemă, resetați Magazinul, goliți memoria cache a Magazinului, apoi rulați depanatorul Windows Update.</span><span class="sxs-lookup"><span data-stu-id="c87c8-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="c87c8-108">Asigurați-vă că Magazinul Microsoft este închis înainte să continuați cu acești pași.</span><span class="sxs-lookup"><span data-stu-id="c87c8-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="c87c8-109">**Pasul 1: Resetați Magazinul Microsoft**</span><span class="sxs-lookup"><span data-stu-id="c87c8-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="c87c8-110">**Rețineți** Acest lucru șterge definitiv datele de aplicație de pe dispozitiv, inclusiv preferințele dvs. și detaliile de conectare.</span><span class="sxs-lookup"><span data-stu-id="c87c8-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="c87c8-111">Selectați **Pornire** > **Setări** > **Aplicații** > **Aplicații și caracteristici**.</span><span class="sxs-lookup"><span data-stu-id="c87c8-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="c87c8-112">În lista de aplicații, găsiți și selectați Magazinul Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c87c8-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="c87c8-113">Selectați **Opțiuni complexe**.</span><span class="sxs-lookup"><span data-stu-id="c87c8-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="c87c8-114">Defilați în jos și selectați **Resetare**, apoi faceți clic **Confirmare resetare**.</span><span class="sxs-lookup"><span data-stu-id="c87c8-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="c87c8-115">**Pasul 2: Goliți memoria cache a Magazinului Microsoft**</span><span class="sxs-lookup"><span data-stu-id="c87c8-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="c87c8-116">Apăsați tasta siglă Windows + R pentru a deschide caseta de dialog Executare.</span><span class="sxs-lookup"><span data-stu-id="c87c8-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="c87c8-117">Tastați wsreset.exe și selectați **OK**.</span><span class="sxs-lookup"><span data-stu-id="c87c8-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="c87c8-118">Se deschide o fereastră Linie de comandă goală.</span><span class="sxs-lookup"><span data-stu-id="c87c8-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="c87c8-119">După aproximativ 10 secunde, fereastra se închide și Magazinul se deschide automat.</span><span class="sxs-lookup"><span data-stu-id="c87c8-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="c87c8-120">**Pasul 3: Resetați Windows Update**</span><span class="sxs-lookup"><span data-stu-id="c87c8-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="c87c8-121">Selectați **Pornire** > **Setări** > **Actualizare și securitate** > **Depanare**.</span><span class="sxs-lookup"><span data-stu-id="c87c8-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="c87c8-122">Defilați în jos și selectați **Windows Update** din listă, apoi selectați **Rulați depanatorul**.</span><span class="sxs-lookup"><span data-stu-id="c87c8-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="c87c8-123">Reporniți-vă computerul și verificați dacă încă vă confruntați cu această problemă.</span><span class="sxs-lookup"><span data-stu-id="c87c8-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

