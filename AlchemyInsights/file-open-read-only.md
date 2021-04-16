---
title: Fișier deschis doar în citire
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813196"
---
# <a name="file-open-read-only"></a><span data-ttu-id="f5732-102">Fișier deschis doar în citire</span><span class="sxs-lookup"><span data-stu-id="f5732-102">File open read-only</span></span>

<span data-ttu-id="f5732-103">Atunci când deschideți fișiere, este posibil să descoperiți că se deschid ca doar în citire.</span><span class="sxs-lookup"><span data-stu-id="f5732-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="f5732-104">În unele cazuri, acest lucru este pentru securitate adăugată, de exemplu, atunci când deschideți fișiere de pe internet, iar alteori, cauza poate fi o setare care poate fi modificată.</span><span class="sxs-lookup"><span data-stu-id="f5732-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="f5732-105">Iată câteva scenarii în care un fișier se deschide ca doar în citire și câțiva pași pe care îi puteți urma pentru a modifica acest lucru.</span><span class="sxs-lookup"><span data-stu-id="f5732-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="f5732-106">**Programul meu antivirus determină ca ele să se deschidă ca doar în citire**</span><span class="sxs-lookup"><span data-stu-id="f5732-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="f5732-107">Unele programe antivirus vă pot proteja împotriva fișierelor potențial nesigure, deschizându-le doar în citire.</span><span class="sxs-lookup"><span data-stu-id="f5732-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="f5732-108">Poate fi necesar să consultați furnizorul dvs. antivirus pentru a afla cum să ajustați aceste setări.</span><span class="sxs-lookup"><span data-stu-id="f5732-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="f5732-109">BitDefender, de exemplu, are conținut despre adăugarea excluderilor pentru aplicații [aici:](https://aka.ms/AA6098i)Cum se adaugă excluderile de aplicații sau procese în Centrul de control BitDefender.</span><span class="sxs-lookup"><span data-stu-id="f5732-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="f5732-110">**Proprietățile fișierului sunt setate la doar în citire?**</span><span class="sxs-lookup"><span data-stu-id="f5732-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="f5732-111">Puteți verifica proprietățile fișierului făcând clic dreapta pe fișier și alegând Proprietăți.</span><span class="sxs-lookup"><span data-stu-id="f5732-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="f5732-112">Dacă este bifat atributul Doar în citire, puteți să îl debifați și să faceți clic pe OK.</span><span class="sxs-lookup"><span data-stu-id="f5732-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="f5732-113">**Conținutul este în vizualizarea protejată**</span><span class="sxs-lookup"><span data-stu-id="f5732-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="f5732-114">Fișierele de pe internet și din alte locații potențial nesigure pot conține viruși, viermi și alte tipuri de malware, care pot dăuna computerului dvs.</span><span class="sxs-lookup"><span data-stu-id="f5732-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="f5732-115">Acest lucru este obișnuit și în cazul atașărilor de e-mail sau al fișierelor pe care le-ați descărcat.</span><span class="sxs-lookup"><span data-stu-id="f5732-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="f5732-116">Pentru a contribui la protejarea computerului, fișierele din aceste locații potențial nesigure se deschid în Vizualizarea protejată.</span><span class="sxs-lookup"><span data-stu-id="f5732-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="f5732-117">Utilizând Vizualizarea protejată, puteți să citiți un fișier și să-i vedeți conținutul, reducând riscurile.</span><span class="sxs-lookup"><span data-stu-id="f5732-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="f5732-118">Pentru mai multe informații despre Vizualizarea protejată și despre cum să modificați setările, consultați acest articol: [Ce este Vizualizarea protejată?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="f5732-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="f5732-119">**OneDrive este plin?**</span><span class="sxs-lookup"><span data-stu-id="f5732-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="f5732-120">Dacă fișierul este stocat în OneDrive și spațiul de stocare OneDrive este plin, nu veți putea să salvați documentul decât după ce rămâneți cu spațiul alocat.</span><span class="sxs-lookup"><span data-stu-id="f5732-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="f5732-121">Puteți să verificați spațiul liber din OneDrive făcând clic pe pictograma OneDrive din centrul de notificare și alegând Gestionați stocarea sau puteți să accesați , să vă conectați și să notați cantitatea de spațiu utilizat în partea din stânga jos a [https://onedrive.live.com](https://onedrive.live.com) ecranului.</span><span class="sxs-lookup"><span data-stu-id="f5732-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="f5732-122">**Office este activat?**</span><span class="sxs-lookup"><span data-stu-id="f5732-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="f5732-123">Dacă Office nu este activat sau dacă abonamentul a expirat, este posibil să fiți în modul de funcționalitate redusă.</span><span class="sxs-lookup"><span data-stu-id="f5732-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="f5732-124">Pentru informații despre cum să activați Office, consultați: Erorile de activare și de produs [nelicențiat în Office.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="f5732-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="f5732-125">**Dacă nimic nu funcționează...**</span><span class="sxs-lookup"><span data-stu-id="f5732-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="f5732-126">Încercați să reporniți computerul</span><span class="sxs-lookup"><span data-stu-id="f5732-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="f5732-127">Instalarea actualizărilor Office</span><span class="sxs-lookup"><span data-stu-id="f5732-127">Install Office updates</span></span>
    
- <span data-ttu-id="f5732-128">Efectuarea unei reparării online a Office</span><span class="sxs-lookup"><span data-stu-id="f5732-128">Perform an Online repair of Office</span></span>
    

