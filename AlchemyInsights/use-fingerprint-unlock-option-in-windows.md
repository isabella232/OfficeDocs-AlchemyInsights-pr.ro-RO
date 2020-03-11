---
title: Utilizarea opțiunii de deblocare a amprentelor digitale în Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588327"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="4e962-102">Utilizarea opțiunii de deblocare a amprentelor digitale în Windows 10</span><span class="sxs-lookup"><span data-stu-id="4e962-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="4e962-103">**Activare amprentă windows hello**</span><span class="sxs-lookup"><span data-stu-id="4e962-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="4e962-104">Pentru a debloca Windows 10 utilizând amprenta, trebuie să configurați Windows Hello Fingerprint adăugând (lăsând Windows să învețe să recunoască) cel puțin un deget.</span><span class="sxs-lookup"><span data-stu-id="4e962-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="4e962-105">Accesați **Setări > conturi > opțiuni de conectare** (sau faceți clic [aici](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="4e962-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="4e962-106">Vor fi listate opțiunile de conectare disponibile.</span><span class="sxs-lookup"><span data-stu-id="4e962-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="4e962-107">De exemplu:</span><span class="sxs-lookup"><span data-stu-id="4e962-107">For example:</span></span>

    ![Opțiuni de conectare.](media/sign-in-options.png)

2. <span data-ttu-id="4e962-109">Faceți clic sau atingeți **Windows Hello Fingerprint**, apoi faceți clic pe **Configurare**.</span><span class="sxs-lookup"><span data-stu-id="4e962-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="4e962-110">În fereastra de configurare Windows Hello, faceți clic pe **Introducere**.</span><span class="sxs-lookup"><span data-stu-id="4e962-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="4e962-111">Senzorul de amprentă se va activa și vi se va cere să plasați degetul pe senzor:</span><span class="sxs-lookup"><span data-stu-id="4e962-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Senzor de amprentă.](media/fingerprint-sensor.png)

3. <span data-ttu-id="4e962-113">Urmați instrucțiunile, care vă vor solicita să scanați în mod repetat degetul.</span><span class="sxs-lookup"><span data-stu-id="4e962-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="4e962-114">Când se termină acest lucru, veți avea opțiunea de a adăuga alte degete pe care doriți să le utilizați pentru conectare.</span><span class="sxs-lookup"><span data-stu-id="4e962-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="4e962-115">Data viitoare când vă conectați la Windows 10, veți avea opțiunea de a utiliza amprenta pentru a face acest lucru.</span><span class="sxs-lookup"><span data-stu-id="4e962-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="4e962-116">**Windows Hello Fingerprint nu este disponibil ca opțiune de conectare**</span><span class="sxs-lookup"><span data-stu-id="4e962-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="4e962-117">Dacă Windows Hello Fingerprint nu este afișat ca opțiune în **opțiunile**de conectare , înseamnă că Windows nu are cunoștință de niciun cititor/scaner de amprente atașat la PC sau că o politică de sistem împiedică utilizarea acestuia (dacă, de exemplu, PC-ul este gestionat de locul de muncă).</span><span class="sxs-lookup"><span data-stu-id="4e962-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="4e962-118">Pentru a depana:</span><span class="sxs-lookup"><span data-stu-id="4e962-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="4e962-119">Selectați butonul **Start** din bara de activități și căutați **Manager dispozitive**.</span><span class="sxs-lookup"><span data-stu-id="4e962-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="4e962-120">Faceți clic sau atingeți pentru a deschide **Manager dispozitive**.</span><span class="sxs-lookup"><span data-stu-id="4e962-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="4e962-121">În Manager dispozitive, extindeți Dispozitive biometrice făcând clic pe simbolul său.</span><span class="sxs-lookup"><span data-stu-id="4e962-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Dispozitive biometrice.](media/biometric-devices.png)

4. <span data-ttu-id="4e962-123">Scanerul de amprente trebuie listat ca dispozitiv biometric, ar fi scanerul Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="4e962-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Dispozitive biometrice.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="4e962-125">Dacă scanerul de amprente nu este afișat și scanerul este integrat în PC, accesați site-ul web al producătorului PC-ului.</span><span class="sxs-lookup"><span data-stu-id="4e962-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="4e962-126">În secțiunea asistență tehnică pentru modelul PC-ului dvs., căutați un driver Windows 10 pentru un scaner pe care îl puteți instala.</span><span class="sxs-lookup"><span data-stu-id="4e962-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="4e962-127">Dacă scanerul este separat de PC (atașat prin USB), accesați site-ul web al producătorului scanerului pentru a găsi și instala software-ul de driver de dispozitiv Windows 10 pentru modelul de scaner pe care îl aveți.</span><span class="sxs-lookup"><span data-stu-id="4e962-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
