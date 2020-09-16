---
title: Setările de pornire în Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751147"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="1864e-102">Setările de pornire în Windows 10</span><span class="sxs-lookup"><span data-stu-id="1864e-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="1864e-103">**Modificarea aplicațiilor care rulează automat la pornire**</span><span class="sxs-lookup"><span data-stu-id="1864e-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="1864e-104">Accesați [setări > aplicații > pornire](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="1864e-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="1864e-105">Asigurați-vă că orice aplicație **pe**care doriți să o difuzați la pornire este activată.</span><span class="sxs-lookup"><span data-stu-id="1864e-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="1864e-106">**Adăugarea unei aplicații pentru rulare automată la pornire**</span><span class="sxs-lookup"><span data-stu-id="1864e-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="1864e-107">Atingeți sau faceți clic pe **Start** și găsiți aplicația pe care doriți să o difuzați la pornire.</span><span class="sxs-lookup"><span data-stu-id="1864e-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="1864e-108">Faceți clic dreapta pe aplicație, faceți clic pe **mai multe**, apoi faceți clic pe **Deschidere locație fișier**.</span><span class="sxs-lookup"><span data-stu-id="1864e-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="1864e-109">Aceasta deschide locația în care se salvează comanda rapidă către aplicație.</span><span class="sxs-lookup"><span data-stu-id="1864e-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="1864e-110">Dacă nu există nicio opțiune pentru locația de fișier deschisă, înseamnă că aplicația nu poate fi executată la pornire.</span><span class="sxs-lookup"><span data-stu-id="1864e-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="1864e-111">Cu locația de fișier deschisă, apăsați **tasta siglă Windows + R**, tastați **Shell: Startup**, apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="1864e-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="1864e-112">Astfel se deschide folderul Startup.</span><span class="sxs-lookup"><span data-stu-id="1864e-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="1864e-113">Copiați și lipiți comanda rapidă către aplicație din locația fișierului în folderul Startup.</span><span class="sxs-lookup"><span data-stu-id="1864e-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="1864e-114">**Opțiuni complexe de pornire (inclusiv modul de siguranță, setările UEFI și pornirea de pe un alt dispozitiv)**</span><span class="sxs-lookup"><span data-stu-id="1864e-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="1864e-115">Salvați-vă lucrul și închideți toate documentele deschise, deoarece acești pași vor reporni PC-ul.</span><span class="sxs-lookup"><span data-stu-id="1864e-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="1864e-116">Accesați [setări > actualizare & securitate > recuperare](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="1864e-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="1864e-117">Sub **pornire complexă**, faceți clic pe **Repornire acum**.</span><span class="sxs-lookup"><span data-stu-id="1864e-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="1864e-118">După ce PC-ul repornește la ecranul Alegeți o opțiune:</span><span class="sxs-lookup"><span data-stu-id="1864e-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="1864e-119">Pentru a porni de pe un dispozitiv, cum ar fi o unitate USB, faceți clic pe **utilizare dispozitiv**.</span><span class="sxs-lookup"><span data-stu-id="1864e-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="1864e-120">Pentru a introduce setările UEFI (numite uneori configurare BIOS), faceți clic pe **Depanarea > opțiuni complexe > setările de firmware UEFI**.</span><span class="sxs-lookup"><span data-stu-id="1864e-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="1864e-121">Pentru a intra în modul de siguranță sau pentru a modifica setările de pornire complexe, faceți clic pe **depanare > opțiuni complexe > setări de pornire**, apoi faceți clic pe **Repornire**.</span><span class="sxs-lookup"><span data-stu-id="1864e-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="1864e-122">Este posibil să vi se solicite să introduceți [cheia de recuperare BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="1864e-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="1864e-123">După repornirea PC-ului, faceți clic pe setarea de pornire pe care doriți să o utilizați.</span><span class="sxs-lookup"><span data-stu-id="1864e-123">After your PC restarts again, click the startup setting you want to use.</span></span>