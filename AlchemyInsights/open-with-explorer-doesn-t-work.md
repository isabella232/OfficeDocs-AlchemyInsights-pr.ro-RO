---
title: Deschidere cu Explorer nu funcţionează
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29484773"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="0e142-102">Deschidere cu Explorer nu este de lucru</span><span class="sxs-lookup"><span data-stu-id="0e142-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="0e142-p101">În cazul în care nu funcţionează **Deschidere cu Explorer** sau **din File Explorer** asiguraţi-vă că serviciul WebClient este setat să **ruleze** urmând paşii de mai jos. De exemplu, ar putea dura mult timp pentru a deschide o bibliotecă SharePoint sau OneDrive, atunci când acest serviciu nu se execută.</span><span class="sxs-lookup"><span data-stu-id="0e142-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="0e142-105">În caseta de căutare Windows, tip alerga, selectaţi app desktop a alerga, tip services.msc, şi apoi selectaţi **Enter**.</span><span class="sxs-lookup"><span data-stu-id="0e142-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="0e142-p102">Derulaţi în jos la serviciu WebClient şi verificaţi coloana de **stare** . În cazul în care starea de service WebClient nu este **rulează**, faceţi dublu clic pe servicii, faceţi clic pe **Start**şi apoi faceţi clic pe **OK**. Activarea serviciului, dacă este necesar, selectând fie **Manual** , fie **automat** în caseta de **tip Startup** .</span><span class="sxs-lookup"><span data-stu-id="0e142-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="0e142-p103">Pentru a depana probleme de deschidere în File Explorer, consultaţi [deschis în Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explora sincronizare ca o alternativă mai bună: [SharePoint sincronizare fişiere cu noul client de sincronizare OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="0e142-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

