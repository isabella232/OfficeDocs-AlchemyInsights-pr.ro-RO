---
title: Depanarea problemelor utilizând deschidere cu Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659070"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="d6ed4-102">Remedierea problemelor cu Explorer deschis</span><span class="sxs-lookup"><span data-stu-id="d6ed4-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="d6ed4-103">Remedierea problemelor obișnuite cu deschiderea unei biblioteci de documente în SharePoint sau OneDrive utilizând comanda **Deschidere cu Explorer** :</span><span class="sxs-lookup"><span data-stu-id="d6ed4-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="d6ed4-104">Utilizați Internet Explorer 10 sau Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="d6ed4-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="d6ed4-105">**Deschiderea cu Explorer** nu este compatibilă cu Microsoft Edge, Google Chrome, Firefox și alții.</span><span class="sxs-lookup"><span data-stu-id="d6ed4-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="d6ed4-106">**Deschiderea cu Explorer** este dezactivată în toate browserele, cu excepția Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="d6ed4-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="d6ed4-107">**Deschiderea cu Explorer** nu este disponibilă în experiența modernă pentru bibliotecile SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d6ed4-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="d6ed4-108">Utilizați **în schimb vizualizarea în Explorer** .</span><span class="sxs-lookup"><span data-stu-id="d6ed4-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="d6ed4-109">Selectați vizualizarea **Opțiuni vizualizare** \> **în Explorer**.</span><span class="sxs-lookup"><span data-stu-id="d6ed4-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="d6ed4-110">Vizualizarea în Explorer nu este compatibilă cu Microsoft Edge, Google Chrome, Firefox și alții.</span><span class="sxs-lookup"><span data-stu-id="d6ed4-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="d6ed4-111">**Vizualizați în Explorer** , disponibil doar în Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="d6ed4-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="d6ed4-112">Asigurați-vă că rulează serviciul de client.</span><span class="sxs-lookup"><span data-stu-id="d6ed4-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="d6ed4-113">În caseta de căutare Windows, tastați rulare, selectați aplicația desktop rulare, tastați Services. msc, apoi apăsați pe Enter.</span><span class="sxs-lookup"><span data-stu-id="d6ed4-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="d6ed4-114">Defilați în jos la serviciul pentru clienți și asigurați-vă că coloana **stare** afișează "rulare".</span><span class="sxs-lookup"><span data-stu-id="d6ed4-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="d6ed4-115">Dacă nu face acest lucru, faceți dublu clic pe serviciu, faceți clic pe **Start**, apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="d6ed4-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="d6ed4-116">(Poate fi necesar să activați mai întâi serviciul selectând fie **manual** , fie **automat** în caseta **tip pornire** .)</span><span class="sxs-lookup"><span data-stu-id="d6ed4-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="d6ed4-117">Deschiderea unei biblioteci în Explorer este utilă dacă trebuie să copiați sau să mutați mai multe fișiere și foldere o singură dată, dar dacă doriți să lucrați în mod regulat în bibliotecă, vă recomandăm să îl sincronizați.</span><span class="sxs-lookup"><span data-stu-id="d6ed4-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="d6ed4-118">Pentru a depana problemele care se deschid în Explorer, consultați [deschiderea în Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="d6ed4-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="d6ed4-119">Pentru informații despre configurarea sincronizării, consultați [sincronizarea fișierelor SharePoint cu noul client de sincronizare OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="d6ed4-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="d6ed4-120">Vă rugăm să consultați articolul [cum să utilizați comanda "deschidere cu Explorer" pentru a depana problemele din SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="d6ed4-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

