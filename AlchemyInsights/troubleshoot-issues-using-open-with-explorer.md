---
title: Depanarea problemelor cu deschidere cu Explorer
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
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759306"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="a3bec-102">Remediați problemele cu deschidere cu Explorer</span><span class="sxs-lookup"><span data-stu-id="a3bec-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="a3bec-103">Remediați problemele comune cu deschiderea o bibliotecă de documente SharePoint sau OneDrive utilizând comanda **Deschidere cu Explorer** :</span><span class="sxs-lookup"><span data-stu-id="a3bec-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="a3bec-104">Utilizarea Internet Explorer 10 sau Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="a3bec-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="a3bec-105">**Deschidere cu Explorer** nu este compatibil cu Microsoft Edge, Google Chrome, Firefox şi altele.</span><span class="sxs-lookup"><span data-stu-id="a3bec-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="a3bec-106">**Deschidere cu Explorer** este dezactivată în toate browserele cu excepția Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="a3bec-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="a3bec-107">**Deschidere cu Explorer** nu este disponibilă în experienţa moderne pentru bibliotecile SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a3bec-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="a3bec-108">Utilizarea **vizualizării în File Explorer** în schimb.</span><span class="sxs-lookup"><span data-stu-id="a3bec-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="a3bec-109">Selectaţi **opţiunile de vizualizare** \> **din File Explorer**.</span><span class="sxs-lookup"><span data-stu-id="a3bec-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="a3bec-110">Din File Explorer nu este compatibil cu Microsoft Edge, Google Chrome, Firefox şi altele.</span><span class="sxs-lookup"><span data-stu-id="a3bec-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="a3bec-111">**Din File Explorer** în disponibilă numai în Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="a3bec-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="a3bec-112">Asiguraţi-vă că se execută serviciul WebClient.</span><span class="sxs-lookup"><span data-stu-id="a3bec-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="a3bec-113">În caseta de căutare Windows, a alerga de tip, selectaţi Run desktop app, tip services.msc, şi apoi apăsaţi Enter.</span><span class="sxs-lookup"><span data-stu-id="a3bec-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="a3bec-114">Derulaţi în jos serviciu WebClient şi asiguraţi-vă că coloana **stare** afişează "Running."</span><span class="sxs-lookup"><span data-stu-id="a3bec-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="a3bec-115">Dacă nu, faceţi dublu clic pe servicii, faceţi clic pe **Start**şi apoi faceţi clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="a3bec-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="a3bec-116">(Trebuie mai întâi să activați serviciul prin selectarea fie **Manual** , fie **automat** în caseta de **tip Startup** .)</span><span class="sxs-lookup"><span data-stu-id="a3bec-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="a3bec-117">O bibliotecă de deschidere în File Explorer este la îndemână dacă aveţi nevoie pentru a copia sau muta mai multe fişiere şi foldere, o dată, dar în cazul în care doriţi să lucraţi în mod regulat în bibliotecă, vă recomandăm sincronizarea-l.</span><span class="sxs-lookup"><span data-stu-id="a3bec-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="a3bec-118">Pentru a depana probleme de deschidere în File Explorer, consultaţi [deschis în Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="a3bec-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="a3bec-119">Pentru informaţii despre configurarea sincronizării, consultaţi [SharePoint sincronizare fişiere cu noul client de sincronizare OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="a3bec-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="a3bec-120">Vă rugăm să consultaţi articolul [cum se utilizează comanda "deschidere cu Explorer" pentru a depana probleme în SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) pentru mai multe informaţii.</span><span class="sxs-lookup"><span data-stu-id="a3bec-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

