---
title: Restricționarea accesului în SharePoint sau OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715896"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="9d726-102">Restricționarea accesului în SharePoint sau OneDrive</span><span class="sxs-lookup"><span data-stu-id="9d726-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="9d726-103">În SharePoint și OneDrive, restricționați accesul la elemente precum fișiere, foldere și liste acordând acces numai la grupurile sau persoanele pe care doriți să le aveți acces.</span><span class="sxs-lookup"><span data-stu-id="9d726-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="9d726-104">În mod implicit, permisiunile în SharePoint sunt moștenite de la mai sus în ierarhie.</span><span class="sxs-lookup"><span data-stu-id="9d726-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="9d726-105">Deci, un fișier moștenire permisiunile sale din folderul, care moștenire permisiunile sale de la bibliotecă, care moștenire permisiunile sale de la site-ul.</span><span class="sxs-lookup"><span data-stu-id="9d726-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="9d726-106">Aveți posibilitatea să partajați la un nivel superior (cum ar fi prin partajarea unui întreg site) și apoi să întrerupeți moștenirea dacă nu doriți să partajați toate elementele de pe site.</span><span class="sxs-lookup"><span data-stu-id="9d726-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="9d726-107">Cu toate acestea, nu recomandăm acest lucru, deoarece face menținerea permisiunilor mai complexe și confuze în viitor.</span><span class="sxs-lookup"><span data-stu-id="9d726-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="9d726-108">Iată ce ai putea face în schimb:</span><span class="sxs-lookup"><span data-stu-id="9d726-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="9d726-109">Dacă, de exemplu, doriți să partajați tot conținutul unui folder, cu excepția unui fișier din el, mutați fișierul respectiv într-o locație nouă care nu este partajată.</span><span class="sxs-lookup"><span data-stu-id="9d726-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="9d726-110">Dacă aveți două subfoldere într-un folder și doriți să partajați un subfolder cu grupurile A și B și să permiteți numai grupa A de acces la al doilea subfolder, partajați folderul părinte cu grupul A și adăugați grupul B la primul subfolder.</span><span class="sxs-lookup"><span data-stu-id="9d726-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="9d726-111">Oprirea partajării unui fișier sau folder</span><span class="sxs-lookup"><span data-stu-id="9d726-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

