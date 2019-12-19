---
title: Depanarea monitorului existent
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738580"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="705f5-102">Depanarea unui monitor existent</span><span class="sxs-lookup"><span data-stu-id="705f5-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="705f5-103">Încercați aceste soluții pentru a depana un monitor.</span><span class="sxs-lookup"><span data-stu-id="705f5-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="705f5-104">**Reîmprospătați ecranul monitorului:**</span><span class="sxs-lookup"><span data-stu-id="705f5-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="705f5-105">Apăsați următoarele taste în același timp: Windows key + Ctrl + Shift + B. Acest lucru va reîmprospăta comunicarea cu driverul grafic.</span><span class="sxs-lookup"><span data-stu-id="705f5-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="705f5-106">Monitoarele tale vor clipi momentan și se întorc după câteva secunde.</span><span class="sxs-lookup"><span data-stu-id="705f5-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="705f5-107">**Depanarea monitorului hardware:**</span><span class="sxs-lookup"><span data-stu-id="705f5-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="705f5-108">Deconectați cablul care conectează PC-ul la monitor și conectați-l la loc.</span><span class="sxs-lookup"><span data-stu-id="705f5-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="705f5-109">Deconectați orice dispozitive neesențiale de pe PC (cum ar fi adaptoare sau docuri).</span><span class="sxs-lookup"><span data-stu-id="705f5-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="705f5-110">**Dacă ați instalat recent o actualizare pe PC, aveți posibilitatea să reveniți la driverul de afișare:**</span><span class="sxs-lookup"><span data-stu-id="705f5-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="705f5-111">Selectați **Start**, tastați **Manager dispozitive**și selectați **Manager dispozitive** din rezultate.</span><span class="sxs-lookup"><span data-stu-id="705f5-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="705f5-112">Extindeți secțiunea **adaptoare de afișare** , faceți clic dreapta pe adaptorul de afișare, ANDS selectați **Proprietăți**.</span><span class="sxs-lookup"><span data-stu-id="705f5-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="705f5-113">Navigați la fila **driver** și selectați **Roll Back Driver**.</span><span class="sxs-lookup"><span data-stu-id="705f5-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="705f5-114">Notă: dacă acest lucru nu este disponibil sau este gri, selectați **nu** din opțiunile de mai jos pentru a trece la pasul următor.</span><span class="sxs-lookup"><span data-stu-id="705f5-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="705f5-115">Poate fi necesar să reporniți PC-ul înainte ca aceste modificări să aibă efect.</span><span class="sxs-lookup"><span data-stu-id="705f5-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="705f5-116">**Dezinstalați și reinstalați driverul de afișare:**</span><span class="sxs-lookup"><span data-stu-id="705f5-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="705f5-117">Selectați **Start**, tastați **Manager dispozitive**și selectați **Manager dispozitive** din rezultate.</span><span class="sxs-lookup"><span data-stu-id="705f5-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="705f5-118">Extindeți secțiunea **adaptoare de afișare** , faceți clic dreapta pe adaptorul de afișare, ANDS selectați **Dezinstalare dispozitiv**.</span><span class="sxs-lookup"><span data-stu-id="705f5-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="705f5-119">Bifați caseta de lângă **ștergerea software-ului de driver pentru acest dispozitiv** și selectați **Dezinstalare**.</span><span class="sxs-lookup"><span data-stu-id="705f5-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="705f5-120">Notă: este posibil să fiți rugat să reporniți computerul în acest stadiu.</span><span class="sxs-lookup"><span data-stu-id="705f5-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="705f5-121">Asigurați-vă că notați instrucțiunile rămase înainte de a reporni.</span><span class="sxs-lookup"><span data-stu-id="705f5-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="705f5-122">Deschideți din nou managerul de dispozitive.</span><span class="sxs-lookup"><span data-stu-id="705f5-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="705f5-123">Extindeți secțiunea **adaptoare de afișare** , faceți clic dreapta pe adaptorul de afișare și selectați **Actualizare driver**.</span><span class="sxs-lookup"><span data-stu-id="705f5-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="705f5-124">Selectați **Căutare automată pentru software-ul de driver de actualizare** și urmați instrucțiunile de instalare.</span><span class="sxs-lookup"><span data-stu-id="705f5-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>