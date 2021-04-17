---
title: Depanarea monitorului existent
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824591"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="4ca33-102">Depanarea unui monitor existent</span><span class="sxs-lookup"><span data-stu-id="4ca33-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="4ca33-103">Încercați aceste soluții pentru a depana un monitor.</span><span class="sxs-lookup"><span data-stu-id="4ca33-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="4ca33-104">**Reîmprospătarea ecranului monitorului:**</span><span class="sxs-lookup"><span data-stu-id="4ca33-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="4ca33-105">Apăsați în același timp următoarele taste: tasta Windows + Ctrl + Shift + B. Astfel, se va reîmprospăta comunicarea cu driverul grafic.</span><span class="sxs-lookup"><span data-stu-id="4ca33-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="4ca33-106">Monitoarele dvs. vor clipi imediat și vor reveni după câteva secunde.</span><span class="sxs-lookup"><span data-stu-id="4ca33-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="4ca33-107">**Depanarea componentelor hardware ale monitorului:**</span><span class="sxs-lookup"><span data-stu-id="4ca33-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="4ca33-108">Deconectați cablul care conectează PC-ul la monitor și conectați-l din nou.</span><span class="sxs-lookup"><span data-stu-id="4ca33-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="4ca33-109">Deconectați toate dispozitivele nee esențiale de la PC (cum ar fi adaptoare sau andocare).</span><span class="sxs-lookup"><span data-stu-id="4ca33-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="4ca33-110">**Dacă ați instalat recent o actualizare pe PC, puteți să reveniți la driverul de afișare:**</span><span class="sxs-lookup"><span data-stu-id="4ca33-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="4ca33-111">Selectați **Start**, **tastați manager dispozitive** și **selectați Manager** dispozitive din rezultate.</span><span class="sxs-lookup"><span data-stu-id="4ca33-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="4ca33-112">Extindeți **secțiunea Plăci video,** faceți clic dreapta pe adaptorul de afișare și selectați **Proprietăți**.</span><span class="sxs-lookup"><span data-stu-id="4ca33-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="4ca33-113">Navigați la fila **Driver** și selectați **Revenire driver**.</span><span class="sxs-lookup"><span data-stu-id="4ca33-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="4ca33-114">Notă: Dacă nu este disponibilă sau este estompată, selectați **Nu** din opțiunile de mai jos pentru a trece la pasul următor.</span><span class="sxs-lookup"><span data-stu-id="4ca33-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="4ca33-115">Poate fi necesar să reporniți PC-ul înainte ca aceste modificări să aibă efect.</span><span class="sxs-lookup"><span data-stu-id="4ca33-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="4ca33-116">**Dezinstalați și reinstalați driverul de afișare:**</span><span class="sxs-lookup"><span data-stu-id="4ca33-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="4ca33-117">Selectați **Start**, **tastați manager dispozitive** și **selectați Manager** dispozitive din rezultate.</span><span class="sxs-lookup"><span data-stu-id="4ca33-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="4ca33-118">Extindeți **secțiunea Plăci video,** faceți clic dreapta pe adaptorul de afișare și selectați **Dezinstalare dispozitiv**.</span><span class="sxs-lookup"><span data-stu-id="4ca33-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="4ca33-119">Bifați caseta de lângă Ștergeți **software-ul de driver pentru acest dispozitiv și** selectați **Dezinstalare**.</span><span class="sxs-lookup"><span data-stu-id="4ca33-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="4ca33-120">Notă: Este posibil să i se solicită să reporniți computerul în această etapă.</span><span class="sxs-lookup"><span data-stu-id="4ca33-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="4ca33-121">Asigurați-vă că scrieți instrucțiunile rămase înainte de a reporni.</span><span class="sxs-lookup"><span data-stu-id="4ca33-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="4ca33-122">Deschideți din nou Manager dispozitive.</span><span class="sxs-lookup"><span data-stu-id="4ca33-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="4ca33-123">Extindeți **secțiunea Plăci video,** faceți clic dreapta pe adaptorul de afișare și selectați **Actualizare driver**.</span><span class="sxs-lookup"><span data-stu-id="4ca33-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="4ca33-124">Selectați **Căutați automat software de actualizare a driverului** și urmați instrucțiunile de instalare.</span><span class="sxs-lookup"><span data-stu-id="4ca33-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>