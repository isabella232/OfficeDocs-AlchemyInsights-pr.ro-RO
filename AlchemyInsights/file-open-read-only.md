---
title: Fișier deschis doar în citire
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745619"
---
# <a name="file-open-read-only"></a><span data-ttu-id="11828-102">Fișier deschis doar în citire</span><span class="sxs-lookup"><span data-stu-id="11828-102">File open read-only</span></span>

<span data-ttu-id="11828-103">Este posibil să descoperiți că, atunci când deschideți fișiere, acestea se deschid doar în citire.</span><span class="sxs-lookup"><span data-stu-id="11828-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="11828-104">În unele cazuri, aceasta este pentru securitate adăugată, cum ar fi atunci când deschideți fișiere de pe Internet și alteori, poate fi cauzată de o setare care poate fi modificată.</span><span class="sxs-lookup"><span data-stu-id="11828-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="11828-105">Iată câteva scenarii în care un fișier deschide doar în citire și câțiva pași pe care îi puteți face pentru a modifica acest lucru.</span><span class="sxs-lookup"><span data-stu-id="11828-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="11828-106">**Antivirusul meu le determină să deschidă doar în citire**</span><span class="sxs-lookup"><span data-stu-id="11828-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="11828-107">Unele programe antivirus vă pot proteja împotriva fișierelor potențial nesigure, deschizându-le doar în citire.</span><span class="sxs-lookup"><span data-stu-id="11828-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="11828-108">Poate fi necesar să consultați furnizorul antivirus pentru a afla cum să ajustați aceste setări.</span><span class="sxs-lookup"><span data-stu-id="11828-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="11828-109">De exemplu, BitDefender are conținut despre adăugarea excluderilor de aplicație aici: [cum se adaugă excluderi de aplicație sau proces în Bitdefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="11828-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="11828-110">**Proprietățile fișierului sunt setate la doar în citire?**</span><span class="sxs-lookup"><span data-stu-id="11828-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="11828-111">Puteți să Verificați proprietățile fișierului dacă faceți clic dreapta pe fișier și alegeți proprietăți.</span><span class="sxs-lookup"><span data-stu-id="11828-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="11828-112">Dacă este bifat atributul doar în citire, puteți să îl debifați și să faceți clic pe OK.</span><span class="sxs-lookup"><span data-stu-id="11828-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="11828-113">**Conținutul este în Vizualizare protejată**</span><span class="sxs-lookup"><span data-stu-id="11828-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="11828-114">Fișierele de pe Internet și din alte locații potențial nesigure pot conține viruși, viermi sau alte tipuri de malware care pot dăuna computerului.</span><span class="sxs-lookup"><span data-stu-id="11828-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="11828-115">Acesta este, de asemenea, de obicei cazul cu atașări de e-mail sau fișiere pe care le-ați descărcat.</span><span class="sxs-lookup"><span data-stu-id="11828-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="11828-116">Pentru a contribui la protejarea computerului, fișierele din aceste locații potențial nesigure sunt deschise în vizualizarea protejată.</span><span class="sxs-lookup"><span data-stu-id="11828-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="11828-117">Prin utilizarea vizualizării protejate, puteți să citiți un fișier și să îi vedeți conținutul în timp ce reduceți riscurile.</span><span class="sxs-lookup"><span data-stu-id="11828-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="11828-118">Pentru mai multe informații despre vizualizarea protejată și despre modificarea setărilor, consultați acest articol: [ce este vizualizarea protejată?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="11828-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="11828-119">**OneDrive este plin?**</span><span class="sxs-lookup"><span data-stu-id="11828-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="11828-120">Dacă fișierul este stocat în OneDrive și spațiul de stocare OneDrive este plin, nu veți putea să salvați documentul până când nu vă aflați sub spațiul alocat.</span><span class="sxs-lookup"><span data-stu-id="11828-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="11828-121">Puteți să vă verificați spațiul liber pe OneDrive făcând clic pe pictograma OneDrive din centrul de notificare și alegând Gestionare stocare sau puteți să accesați, să [https://onedrive.live.com](https://onedrive.live.com) vă conectați și să notați cantitatea de spațiu utilizat în partea din stânga jos a ecranului.</span><span class="sxs-lookup"><span data-stu-id="11828-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="11828-122">**Office este activat?**</span><span class="sxs-lookup"><span data-stu-id="11828-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="11828-123">Dacă Office nu este activat sau dacă abonamentul a expirat, ați putea fi în modul de funcționalitate redusă doar în citire.</span><span class="sxs-lookup"><span data-stu-id="11828-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="11828-124">Pentru informații despre cum să activați Office, consultați: [produs nelicențiat și erori de activare în Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="11828-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="11828-125">**Dacă toate celelalte nu reușesc...**</span><span class="sxs-lookup"><span data-stu-id="11828-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="11828-126">Încercați să reporniți computerul</span><span class="sxs-lookup"><span data-stu-id="11828-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="11828-127">Instalarea actualizărilor Office</span><span class="sxs-lookup"><span data-stu-id="11828-127">Install Office updates</span></span>
    
- <span data-ttu-id="11828-128">Efectuarea unei reparații online de Office</span><span class="sxs-lookup"><span data-stu-id="11828-128">Perform an Online repair of Office</span></span>
    

