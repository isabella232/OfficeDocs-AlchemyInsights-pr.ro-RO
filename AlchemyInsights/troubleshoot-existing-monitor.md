---
title: Depanarea monitorului existent
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690723"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="54426-102">Depanarea unui monitor existent</span><span class="sxs-lookup"><span data-stu-id="54426-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="54426-103">Încercați aceste soluții pentru a depana un monitor.</span><span class="sxs-lookup"><span data-stu-id="54426-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="54426-104">**Reîmprospătați ecranul monitorului:**</span><span class="sxs-lookup"><span data-stu-id="54426-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="54426-105">Apăsați simultan tastele următoare: tasta Windows + Ctrl + Shift + B. Aceasta va reîmprospăta comunicarea cu driverul grafic.</span><span class="sxs-lookup"><span data-stu-id="54426-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="54426-106">Monitoarele dumneavoastră vor clipi imediat și revin după câteva secunde.</span><span class="sxs-lookup"><span data-stu-id="54426-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="54426-107">**Depanarea hardware-ului monitorului:**</span><span class="sxs-lookup"><span data-stu-id="54426-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="54426-108">Deconectați cablul la conectarea PC-ului la monitor și conectați-l din nou.</span><span class="sxs-lookup"><span data-stu-id="54426-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="54426-109">Deconectați toate dispozitivele neesențiale de pe PC (cum ar fi adaptoare sau docuri).</span><span class="sxs-lookup"><span data-stu-id="54426-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="54426-110">**Dacă ați instalat recent o actualizare pe PC, puteți să reveniți la driverul de afișare:**</span><span class="sxs-lookup"><span data-stu-id="54426-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="54426-111">Selectați **Start**, tastați **Manager dispozitive**și selectați **Manager dispozitive** din rezultate.</span><span class="sxs-lookup"><span data-stu-id="54426-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="54426-112">Extindeți secțiunea **adaptoare de afișare** , faceți clic cu butonul din dreapta pe adaptorul de afișare, selectați **Proprietăți**.</span><span class="sxs-lookup"><span data-stu-id="54426-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="54426-113">Navigați la fila **driver** și selectați **driver roll back**.</span><span class="sxs-lookup"><span data-stu-id="54426-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="54426-114">Notă: dacă acest lucru nu este disponibil sau este estompat, selectați **nu** din opțiunile de mai jos pentru a trece la pasul următor.</span><span class="sxs-lookup"><span data-stu-id="54426-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="54426-115">Poate fi necesar să reporniți PC-ul înainte ca aceste modificări să aibă efect.</span><span class="sxs-lookup"><span data-stu-id="54426-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="54426-116">**Dezinstalați și reinstalați driverul de afișare:**</span><span class="sxs-lookup"><span data-stu-id="54426-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="54426-117">Selectați **Start**, tastați **Manager dispozitive**și selectați **Manager dispozitive** din rezultate.</span><span class="sxs-lookup"><span data-stu-id="54426-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="54426-118">Extindeți secțiunea **adaptoare de afișare** , faceți clic cu butonul din dreapta pe adaptorul de afișare, selectați **Dezinstalare dispozitiv**.</span><span class="sxs-lookup"><span data-stu-id="54426-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="54426-119">Bifați caseta de lângă **Ștergeți software-ul de driver pentru acest dispozitiv** și selectați **Dezinstalare**.</span><span class="sxs-lookup"><span data-stu-id="54426-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="54426-120">Notă: este posibil să vi se solicite să reporniți computerul în acest moment.</span><span class="sxs-lookup"><span data-stu-id="54426-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="54426-121">Asigurați-vă că scrieți instrucțiunile rămase înainte de a reporni.</span><span class="sxs-lookup"><span data-stu-id="54426-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="54426-122">Deschideți din nou Device Manager.</span><span class="sxs-lookup"><span data-stu-id="54426-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="54426-123">Extindeți secțiunea **adaptoare de afișare** , faceți clic cu butonul din dreapta pe adaptorul de afișare și selectați **actualizați driverul**.</span><span class="sxs-lookup"><span data-stu-id="54426-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="54426-124">Selectați **Căutare automată pentru actualizare software de driver** și urmați instrucțiunile de instalare.</span><span class="sxs-lookup"><span data-stu-id="54426-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>