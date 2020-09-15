---
title: Deschiderea cu Explorer nu funcționează
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694468"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="00a67-102">Deschiderea cu Explorer nu funcționează</span><span class="sxs-lookup"><span data-stu-id="00a67-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="00a67-103">Dacă **deschiderea cu Explorer** sau **vizualizarea în Explorer** nu funcționează, asigurați-vă că serviciul pentru clienți este setat la **rulare** urmând pașii de mai jos.</span><span class="sxs-lookup"><span data-stu-id="00a67-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="00a67-104">De exemplu, poate dura mult timp pentru a deschide o bibliotecă SharePoint sau OneDrive atunci când serviciul nu rulează.</span><span class="sxs-lookup"><span data-stu-id="00a67-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="00a67-105">În caseta de căutare Windows, tastați rulare, selectați aplicația desktop rulare, tastați Services. msc, apoi selectați **Enter**.</span><span class="sxs-lookup"><span data-stu-id="00a67-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="00a67-106">Defilați în jos la serviciul pentru clienți și verificați coloana **stare** .</span><span class="sxs-lookup"><span data-stu-id="00a67-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="00a67-107">Dacă starea serviciului client nu **rulează**, faceți dublu clic pe serviciu, faceți clic pe **Start**, apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="00a67-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="00a67-108">Activați serviciul, dacă este necesar, selectând fie **manual** , fie **automat** în caseta **tip lansare** în execuție.</span><span class="sxs-lookup"><span data-stu-id="00a67-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="00a67-109">Pentru a depana problemele care se deschid în Explorer, consultați [deschiderea în Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="00a67-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="00a67-110">Explorați sincronizarea ca alternativă mai bună: [Sincronizați fișierele SharePoint cu noul client de sincronizare OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="00a67-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

