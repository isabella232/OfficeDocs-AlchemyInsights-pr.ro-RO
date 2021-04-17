---
title: Setări de pornire în Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828164"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="f037e-102">Setări de pornire în Windows 10</span><span class="sxs-lookup"><span data-stu-id="f037e-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="f037e-103">**Modificați aplicațiile care rulează automat la pornire**</span><span class="sxs-lookup"><span data-stu-id="f037e-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="f037e-104">Accesați Setări [> Apps > Pornire](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="f037e-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="f037e-105">Asigurați-vă că orice aplicație pe care doriți să rulați la pornire este **activată.**</span><span class="sxs-lookup"><span data-stu-id="f037e-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="f037e-106">**Adăugarea unei aplicații pentru a rula automat la pornire**</span><span class="sxs-lookup"><span data-stu-id="f037e-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="f037e-107">Atingeți sau faceți **clic pe Start** și găsiți aplicația pe care doriți să o rulați la pornire.</span><span class="sxs-lookup"><span data-stu-id="f037e-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="f037e-108">Faceți clic dreapta pe aplicație, faceți clic **pe Mai** multe , apoi faceți clic pe Deschidere **locație fișier.**</span><span class="sxs-lookup"><span data-stu-id="f037e-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="f037e-109">Aceasta deschide locația unde este salvată comanda rapidă la aplicație.</span><span class="sxs-lookup"><span data-stu-id="f037e-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="f037e-110">Dacă nu există nicio opțiune pentru Deschidere locație fișier, înseamnă că aplicația nu poate rula la pornire.</span><span class="sxs-lookup"><span data-stu-id="f037e-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="f037e-111">Cu locația fișierului deschisă, apăsați **tasta siglă Windows + R**, tastați **shell:startup**, apoi faceți clic **pe OK**.</span><span class="sxs-lookup"><span data-stu-id="f037e-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="f037e-112">Astfel se deschide folderul Pornire.</span><span class="sxs-lookup"><span data-stu-id="f037e-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="f037e-113">Copiați și lipiți comanda rapidă la aplicație din locația fișierului în folderul Pornire.</span><span class="sxs-lookup"><span data-stu-id="f037e-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="f037e-114">**Opțiuni de pornire complexe (inclusiv Modul de siguranță, setările UEFI și pornirea de pe un alt dispozitiv)**</span><span class="sxs-lookup"><span data-stu-id="f037e-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="f037e-115">Salvați-vă lucrul și închideți toate documentele deschise, deoarece acești pași vor reporni PC-ul.</span><span class="sxs-lookup"><span data-stu-id="f037e-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="f037e-116">Accesați Setări [> Recuperare & securitate > actualizare.](ms-settings:recovery?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="f037e-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="f037e-117">Sub Pornire **complexă, faceți** clic **pe Repornire acum.**</span><span class="sxs-lookup"><span data-stu-id="f037e-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="f037e-118">După ce PC-ul repornește pe ecranul Alegeți o opțiune:</span><span class="sxs-lookup"><span data-stu-id="f037e-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="f037e-119">Pentru a porni de pe un dispozitiv, cum ar fi o unitate USB, faceți **clic pe Utilizați un dispozitiv**.</span><span class="sxs-lookup"><span data-stu-id="f037e-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="f037e-120">Pentru a introduce setările UEFI (denumite uneori configurare FIS), faceți clic **pe > opțiuni complexe > setările firmware UEFI.**</span><span class="sxs-lookup"><span data-stu-id="f037e-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="f037e-121">Pentru a intra în Modul de siguranță sau a modifica setările de pornire complexe, faceți clic pe > opțiuni complexe **> pornire,** apoi faceți clic pe **Repornire.**</span><span class="sxs-lookup"><span data-stu-id="f037e-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="f037e-122">Este posibil să fiți solicitat să introduceți [cheia de recuperare BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="f037e-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="f037e-123">După ce PC-ul repornește, faceți clic pe setarea de pornire pe care doriți să o utilizați.</span><span class="sxs-lookup"><span data-stu-id="f037e-123">After your PC restarts again, click the startup setting you want to use.</span></span>