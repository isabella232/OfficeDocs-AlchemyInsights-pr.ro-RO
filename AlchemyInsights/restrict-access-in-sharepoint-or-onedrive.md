---
title: Restricționați accesul în SharePoint sau OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551463"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="967e1-102">Restricționați accesul în SharePoint sau OneDrive</span><span class="sxs-lookup"><span data-stu-id="967e1-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="967e1-103">În SharePoint și OneDrive, Restricționați accesul la elemente ar fi fișiere, foldere și liste prin acordarea accesului numai la grupuri sau persoane pe care doriți să aveți acces.</span><span class="sxs-lookup"><span data-stu-id="967e1-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="967e1-104">În mod implicit, permisiunile în SharePoint sunt moștenite de sus în ierarhia.</span><span class="sxs-lookup"><span data-stu-id="967e1-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="967e1-105">Deci, un fișier moșteneste permisiunile sale din folderul, care moșteneste permisiunile sale de la biblioteca, care moșteneste permisiunile sale de la site-ul.</span><span class="sxs-lookup"><span data-stu-id="967e1-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="967e1-106">Puteți partaja la un nivel mai înalt (cum ar fi prin partajarea unui întreg site) și apoi rupe moștenirea dacă nu doriți să partajați toate elementele de pe site-ul.</span><span class="sxs-lookup"><span data-stu-id="967e1-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="967e1-107">Cu toate acestea, nu recomandăm acest lucru, deoarece face menținerea permisiunile mai complexe și confuze în viitor.</span><span class="sxs-lookup"><span data-stu-id="967e1-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="967e1-108">Iată ce ai putea face în schimb:</span><span class="sxs-lookup"><span data-stu-id="967e1-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="967e1-109">Dacă, de exemplu, doriți să partajați tot conținutul unui folder, cu excepția unui fișier din acesta, mutați fișierul într-o locație nouă care nu este partajată.</span><span class="sxs-lookup"><span data-stu-id="967e1-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="967e1-110">Dacă aveți două subfoldere într-un folder și doriți să partajați un subfolder cu grupurile A și B și să permiteți numai grupului A acces la al doilea subfolder, partajați folderul părinte cu grupul A și adăugați Grupa B la primul subfolder.</span><span class="sxs-lookup"><span data-stu-id="967e1-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="967e1-111">Oprirea partajării unui fișier sau a unui folder</span><span class="sxs-lookup"><span data-stu-id="967e1-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

