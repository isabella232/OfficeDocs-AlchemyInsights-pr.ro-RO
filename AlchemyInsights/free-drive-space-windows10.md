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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037946"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="a6ea1-102">Eliberați spațiu pe disc în Windows 10</span><span class="sxs-lookup"><span data-stu-id="a6ea1-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="a6ea1-103">Iată două opțiuni pentru a elibera spațiu pe hard disk în Windows:</span><span class="sxs-lookup"><span data-stu-id="a6ea1-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="a6ea1-104">Eliberați spațiu pe disc în Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="a6ea1-105">Eliberați spațiu pentru actualizările Windows 10 cu dispozitivul de stocare extern.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="a6ea1-106">Dacă încă aveți spațiu-disc redus după ce utilizați Curățare disc, este posibil ca folderul temp să se completeze rapid cu fișiere de aplicație (. imbinare) utilizate de Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="a6ea1-107">Pentru a remedia această problemă, resetați magazinul, debifați memoria cache a magazinului, apoi rulează depanatorul Windows Update.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="a6ea1-108">Asigurați-vă că Microsoft Store este închis înainte de a continua cu acești pași.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="a6ea1-109">**Pasul 1: reinițializați Magazinul Microsoft**</span><span class="sxs-lookup"><span data-stu-id="a6ea1-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="a6ea1-110">**Notă** Acest lucru șterge definitiv datele aplicației pe dispozitiv, inclusiv preferințele și detaliile de conectare.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="a6ea1-111">Selectați   >  **Setări** pornire aplicații  >  **aplicații**  >  **& caracteristici**.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="a6ea1-112">În lista de aplicații, găsiți și selectați Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="a6ea1-113">Selectați **Opțiuni complexe**.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="a6ea1-114">Defilați în jos și selectați **Reinițializare**, apoi **confirmați resetare**.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="a6ea1-115">**Pasul 2: debifați memoria cache a magazinului Microsoft**</span><span class="sxs-lookup"><span data-stu-id="a6ea1-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="a6ea1-116">Apăsați tasta siglă Windows + R pentru a deschide caseta de dialog rulare.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="a6ea1-117">Tastați wsreset.exe și selectați **OK**.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="a6ea1-118">Se deschide o fereastră de linie de comandă necompletată.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="a6ea1-119">După aproximativ 10 secunde, se închide fereastra, iar magazinul se deschide automat.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="a6ea1-120">**Pasul 3: Resetarea Windows Update**</span><span class="sxs-lookup"><span data-stu-id="a6ea1-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="a6ea1-121">Selectați   >  Actualizare **Setări** pornire  >  **& depanare de securitate**  >  .</span><span class="sxs-lookup"><span data-stu-id="a6ea1-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="a6ea1-122">Defilați în jos și selectați **Windows Update** din listă și selectați **rulare depanatorul**.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="a6ea1-123">Reporniți computerul și verificați dacă încă întâmpinați problema.</span><span class="sxs-lookup"><span data-stu-id="a6ea1-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

