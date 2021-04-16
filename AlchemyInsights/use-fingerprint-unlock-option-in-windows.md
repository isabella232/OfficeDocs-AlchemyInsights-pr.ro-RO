---
title: Utilizarea opțiunii de deblocare a amprentelor în Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796689"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="60717-102">Utilizarea opțiunii de deblocare a amprentelor în Windows 10</span><span class="sxs-lookup"><span data-stu-id="60717-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="60717-103">**Activarea amprentelor Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="60717-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="60717-104">Pentru a debloca Windows 10 folosind amprenta, trebuie să configurați amprentă Windows Hello adăugând (permițând ca Windows să învețe să recunoască) cel puțin un deget.</span><span class="sxs-lookup"><span data-stu-id="60717-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="60717-105">Accesați Setări **> Conturi > Opțiuni de conectare (sau faceți** clic [aici](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="60717-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="60717-106">Vor fi listate opțiunile disponibile de conectare.</span><span class="sxs-lookup"><span data-stu-id="60717-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="60717-107">De exemplu:</span><span class="sxs-lookup"><span data-stu-id="60717-107">For example:</span></span>

    ![Opțiuni de conectare.](media/sign-in-options.png)

2. <span data-ttu-id="60717-109">Faceți clic sau **atingeți Amprentă Windows Hello**, apoi faceți clic pe **Instalare**.</span><span class="sxs-lookup"><span data-stu-id="60717-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="60717-110">În fereastra de instalare Windows Hello, faceți **clic pe Incepeți.**</span><span class="sxs-lookup"><span data-stu-id="60717-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="60717-111">Senzorul de amprente se va activa și veți fi întrebat dacă puneți degetul pe senzor:</span><span class="sxs-lookup"><span data-stu-id="60717-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Senzor de amprente.](media/fingerprint-sensor.png)

3. <span data-ttu-id="60717-113">Urmați instrucțiunile, care vă vor solicita să scanați în mod repetat cu degetul.</span><span class="sxs-lookup"><span data-stu-id="60717-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="60717-114">Când se termină aceasta, veți avea opțiunea de a adăuga alte degete pe care poate doriți să le utilizați pentru conectare.</span><span class="sxs-lookup"><span data-stu-id="60717-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="60717-115">Data viitoare când vă conectați la Windows 10, veți avea opțiunea de a utiliza amprenta pentru a face acest lucru.</span><span class="sxs-lookup"><span data-stu-id="60717-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="60717-116">**Amprentă Windows Hello nu este disponibilă ca opțiune de conectare**</span><span class="sxs-lookup"><span data-stu-id="60717-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="60717-117">Dacă amprentă Windows Hello nu este afișată ca opțiune de opțiuni de conectare, înseamnă că Windows nu cunoaște niciun cititor de amprente sau scaner atașat la PC sau că o politică de sistem împiedică utilizarea acesteia (de exemplu, **PC-ul** este gestionat de locul de muncă).</span><span class="sxs-lookup"><span data-stu-id="60717-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="60717-118">Pentru a depana:</span><span class="sxs-lookup"><span data-stu-id="60717-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="60717-119">Selectați **butonul Start** din bara de activități și căutați Manager **dispozitive**.</span><span class="sxs-lookup"><span data-stu-id="60717-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="60717-120">Atingeți sau faceți clic pentru a **deschide Manager dispozitive**.</span><span class="sxs-lookup"><span data-stu-id="60717-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="60717-121">În Manager dispozitive, extindeți Dispozitivele biometrice, făcând clic pe ghilimelele unghiulare.</span><span class="sxs-lookup"><span data-stu-id="60717-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Dispozitive biometrice.](media/biometric-devices.png)

4. <span data-ttu-id="60717-123">Scanerul de amprente ar trebui să fie listat ca dispozitiv biometric, cum ar fi scanerul de sindicalizare WBDI:</span><span class="sxs-lookup"><span data-stu-id="60717-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Dispozitive biometrice.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="60717-125">Dacă scanerul de amprente nu este afișat și scanerul este integrat în PC, accesați site-ul web al producătorului PC-ului.</span><span class="sxs-lookup"><span data-stu-id="60717-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="60717-126">În secțiunea de asistență tehnică pentru modelul PC, căutați un driver Windows 10 pentru un scaner pe care să îl puteți instala.</span><span class="sxs-lookup"><span data-stu-id="60717-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="60717-127">Dacă scanerul este separat de PC (atașat prin USB), accesați site-ul web al producătorului scanerului pentru a găsi și a instala software-ul de driver de dispozitiv Windows 10 pentru modelul de scaner pe care îl aveți.</span><span class="sxs-lookup"><span data-stu-id="60717-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
