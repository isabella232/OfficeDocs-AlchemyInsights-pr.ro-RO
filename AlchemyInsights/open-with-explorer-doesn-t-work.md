---
title: Deschiderea cu Explorer nu funcționează
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713046"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="756d1-102">Deschiderea cu Explorer nu funcționează</span><span class="sxs-lookup"><span data-stu-id="756d1-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="756d1-103">Dacă **Deschidere cu Explorer** sau Vizualizare în **Explorer** nu funcționează, asigurați-vă că serviciul WebClient este setat la **Executare** urmând pașii de mai jos.</span><span class="sxs-lookup"><span data-stu-id="756d1-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="756d1-104">De exemplu, poate dura mult timp pentru a deschide o bibliotecă SharePoint sau OneDrive atunci când serviciul nu se execută.</span><span class="sxs-lookup"><span data-stu-id="756d1-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="756d1-105">În caseta de căutare Windows, tastați executare, selectați aplicația Executare desktop, tastați services.msc, apoi **selectați Enter**.</span><span class="sxs-lookup"><span data-stu-id="756d1-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="756d1-106">Defilați în jos la serviciul WebClient și verificați coloana **Stare.**</span><span class="sxs-lookup"><span data-stu-id="756d1-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="756d1-107">Dacă starea serviciului WebClient nu **se execută**, faceți dublu clic pe serviciu, faceți clic pe **Start**, apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="756d1-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="756d1-108">Activați serviciul, dacă este necesar, selectând **Manual** sau **Automat** în caseta **Tip pornire.**</span><span class="sxs-lookup"><span data-stu-id="756d1-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="756d1-109">Pentru a depana problemele de deschidere în Explorer, consultați [Deschiderea în Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="756d1-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="756d1-110">Explorați sincronizarea ca alternativă mai bună: [sincronizați fișierele SharePoint cu noul client de sincronizare OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="756d1-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

