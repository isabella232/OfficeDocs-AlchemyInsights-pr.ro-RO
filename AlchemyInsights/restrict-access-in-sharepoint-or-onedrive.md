---
title: Restricționarea accesului în SharePoint sau OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720694"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="574fa-102">Restricționarea accesului în SharePoint sau OneDrive</span><span class="sxs-lookup"><span data-stu-id="574fa-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="574fa-103">În SharePoint și OneDrive, Restricționați accesul la elemente cum ar fi fișiere, foldere și liste, acordând acces doar grupurilor sau persoanelor care doriți să aibă acces.</span><span class="sxs-lookup"><span data-stu-id="574fa-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="574fa-104">În mod implicit, permisiunile din SharePoint sunt moștenite de la mai sus în ierarhie.</span><span class="sxs-lookup"><span data-stu-id="574fa-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="574fa-105">Prin urmare, un fișier își moștenește permisiunile din folder, care îi moștenește permisiunile din bibliotecă, care îi moștenește permisiunile de pe site.</span><span class="sxs-lookup"><span data-stu-id="574fa-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="574fa-106">Puteți să partajați la un nivel mai înalt (de exemplu, prin partajarea unui site întreg), apoi să întrerupeți moștenirea dacă nu doriți să partajați toate elementele de pe site.</span><span class="sxs-lookup"><span data-stu-id="574fa-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="574fa-107">Cu toate acestea, nu recomandăm acest lucru deoarece face menținerea permisiunilor mai complexe și mai confuze în viitor.</span><span class="sxs-lookup"><span data-stu-id="574fa-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="574fa-108">Iată ce puteți face în schimb:</span><span class="sxs-lookup"><span data-stu-id="574fa-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="574fa-109">Dacă, de exemplu, doriți să partajați tot conținutul unui folder, cu excepția unui fișier din acesta, mutați acel fișier într-o locație nouă care nu este partajată.</span><span class="sxs-lookup"><span data-stu-id="574fa-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="574fa-110">Dacă aveți două subfoldere într-un folder și doriți să partajați un subfolder cu grupurile A și B și să permiteți gruparea unui acces la cel de-al doilea subfolder, partajați folderul părinte cu grupul A și adăugați grupul B la primul subfolder.</span><span class="sxs-lookup"><span data-stu-id="574fa-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="574fa-111">Oprirea partajării unui fișier sau folder </span><span class="sxs-lookup"><span data-stu-id="574fa-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

