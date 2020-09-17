---
title: Opțiunea de a utiliza deblocarea amprentelor în Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795256"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="e1f4f-102">Opțiunea de a utiliza deblocarea amprentelor în Windows 10</span><span class="sxs-lookup"><span data-stu-id="e1f4f-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="e1f4f-103">**Activare amprentă Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="e1f4f-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="e1f4f-104">Pentru a debloca Windows 10 utilizând amprenta, trebuie să configurați amprenta Windows Hello prin Adăugare (permițând Windows să învețe să recunoască) cel puțin un deget.</span><span class="sxs-lookup"><span data-stu-id="e1f4f-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="e1f4f-105">Accesați **setări > conturi > opțiuni de conectare** (sau faceți clic [aici](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="e1f4f-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="e1f4f-106">Opțiunile de conectare disponibile vor fi listate.</span><span class="sxs-lookup"><span data-stu-id="e1f4f-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="e1f4f-107">De exemplu:</span><span class="sxs-lookup"><span data-stu-id="e1f4f-107">For example:</span></span>

    ![Opțiuni de conectare.](media/sign-in-options.png)

2. <span data-ttu-id="e1f4f-109">Atingeți sau faceți clic pe **Windows Hello amprentă**, apoi faceți clic pe **configurare**.</span><span class="sxs-lookup"><span data-stu-id="e1f4f-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="e1f4f-110">În fereastra de configurare Windows Hello **, faceți clic pe introducere.**</span><span class="sxs-lookup"><span data-stu-id="e1f4f-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="e1f4f-111">Senzorul de amprentă va fi activat și vi se va solicita să puneți degetul pe senzor:</span><span class="sxs-lookup"><span data-stu-id="e1f4f-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Senzor de amprentă.](media/fingerprint-sensor.png)

3. <span data-ttu-id="e1f4f-113">Urmați instrucțiunile, care vă vor solicita să scanați în mod repetat degetul.</span><span class="sxs-lookup"><span data-stu-id="e1f4f-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="e1f4f-114">Când se termină acest lucru, veți avea opțiunea de a adăuga alte degete pe care poate doriți să le utilizați pentru conectare.</span><span class="sxs-lookup"><span data-stu-id="e1f4f-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="e1f4f-115">Data viitoare când vă conectați la Windows 10, veți avea opțiunea de a vă folosi amprenta pentru a face acest lucru.</span><span class="sxs-lookup"><span data-stu-id="e1f4f-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="e1f4f-116">**Amprenta Windows Hello nu este disponibilă ca opțiune de conectare**</span><span class="sxs-lookup"><span data-stu-id="e1f4f-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="e1f4f-117">Dacă amprenta digitală din Windows Hello nu este afișată ca opțiune în **opțiunile de conectare**, înseamnă că Windows nu este conștient de niciun cititor de amprente/scaner ATAȘAT la PC sau că o politică de sistem îi împiedică utilizarea (dacă, de exemplu, PC-ul este gestionat de locul de muncă).</span><span class="sxs-lookup"><span data-stu-id="e1f4f-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="e1f4f-118">Pentru a depana:</span><span class="sxs-lookup"><span data-stu-id="e1f4f-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="e1f4f-119">Selectați butonul **Start** în bara de activități și căutați **Manager dispozitive**.</span><span class="sxs-lookup"><span data-stu-id="e1f4f-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="e1f4f-120">Faceți clic sau atingeți pentru a deschide **Manager dispozitive**.</span><span class="sxs-lookup"><span data-stu-id="e1f4f-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="e1f4f-121">În Manager dispozitive, extindeți dispozitivele biometrice făcând clic pe ghilimelele sale.</span><span class="sxs-lookup"><span data-stu-id="e1f4f-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Dispozitive biometrice.](media/biometric-devices.png)

4. <span data-ttu-id="e1f4f-123">Scanerul de amprente trebuie să fie listat ca dispozitiv biometric, cum ar fi scanerul Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="e1f4f-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Dispozitive biometrice.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="e1f4f-125">Dacă scanerul de amprente nu este afișat și scanerul este integrat în PC-ul dvs., accesați site-ul web al producătorului PC-ului.</span><span class="sxs-lookup"><span data-stu-id="e1f4f-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="e1f4f-126">În secțiunea asistență tehnică pentru modelul PC-ului, căutați un driver Windows 10 pentru un scaner pe care îl puteți instala.</span><span class="sxs-lookup"><span data-stu-id="e1f4f-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="e1f4f-127">Dacă scanerul este separat de PC (atașat prin USB), accesați site-ul web al producătorului scanerului pentru a găsi și a instala software de driver de dispozitiv Windows 10 pentru modelul de scaner pe care îl aveți.</span><span class="sxs-lookup"><span data-stu-id="e1f4f-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
