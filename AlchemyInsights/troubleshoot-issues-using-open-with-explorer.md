---
title: Depanarea problemelor utilizând deschidere cu Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742745"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="a5b81-102">Remediați problemele cu deschidere cu Explorer</span><span class="sxs-lookup"><span data-stu-id="a5b81-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="a5b81-103">Remediați problemele obișnuite cu deschiderea unei biblioteci de documente în SharePoint sau OneDrive utilizând comanda **Deschidere cu Explorer** :</span><span class="sxs-lookup"><span data-stu-id="a5b81-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="a5b81-104">Utilizați Internet Explorer 10 sau Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="a5b81-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="a5b81-105">**Deschiderea cu Explorer** nu este compatibilă cu Microsoft Edge, Google Chrome, Firefox și alții.</span><span class="sxs-lookup"><span data-stu-id="a5b81-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="a5b81-106">**Deschis cu Explorer** este dezactivat în toate browserele, cu excepția Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="a5b81-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="a5b81-107">**Deschidere cu Explorer** nu este disponibilă în experiența modernă pentru bibliotecile SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5b81-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="a5b81-108">Utilizați **vizualizare în Explorer în** schimb.</span><span class="sxs-lookup"><span data-stu-id="a5b81-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="a5b81-109">Selectați vizualizare **Opțiuni** \> vizualizare **în Explorer**.</span><span class="sxs-lookup"><span data-stu-id="a5b81-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="a5b81-110">Vizualizarea în File Explorer nu este compatibilă cu Microsoft Edge, Google Chrome, Firefox și alții.</span><span class="sxs-lookup"><span data-stu-id="a5b81-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="a5b81-111">**Vizualizare în Explorer** disponibil numai în Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="a5b81-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="a5b81-112">Asigurați-vă că serviciul WebClient se execută.</span><span class="sxs-lookup"><span data-stu-id="a5b81-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="a5b81-113">În caseta de căutare Windows, tastați Run, selectați aplicația executare desktop, tastați Services. msc, apoi apăsați Enter.</span><span class="sxs-lookup"><span data-stu-id="a5b81-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="a5b81-114">Derulați în jos la serviciul WebClient și asigurați-vă că coloana de **stare** afișează "running".</span><span class="sxs-lookup"><span data-stu-id="a5b81-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="a5b81-115">Dacă nu, faceți dublu clic pe serviciu, faceți clic pe **Start**, apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="a5b81-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="a5b81-116">(Este posibil să fie necesar să activați mai întâi serviciul selectând **manual** sau **automat** în caseta **tip Startup** .)</span><span class="sxs-lookup"><span data-stu-id="a5b81-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="a5b81-117">Deschiderea unei biblioteci în Explorer este utilă dacă trebuie să copiați sau să mutați mai multe fișiere și foldere o dată, dar dacă doriți să lucrați în mod regulat în bibliotecă, vă recomandăm să o sincronizați.</span><span class="sxs-lookup"><span data-stu-id="a5b81-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="a5b81-118">Pentru a depana problemele de deschidere în Explorer, consultați [Deschidere în Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="a5b81-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="a5b81-119">Pentru informații despre configurarea sincronizării, consultați [sincronizarea fișierelor SharePoint cu noul client de sincronizare OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="a5b81-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="a5b81-120">Vă rugăm să consultați articolul [se utilizează comanda deschidere cu Explorer pentru a depana probleme în SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="a5b81-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

